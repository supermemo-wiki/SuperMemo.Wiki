---
title: Backup Strategy Guide
description: 
published: true
date: 2020-12-06T22:29:04.012Z
tags: 
editor: markdown
dateCreated: 2020-12-06T14:16:06.567Z
---

# Why & How ?

## Why should you backup ?

> ⚠️ **Your collection is precious**. If you are using SuperMemo, you will likely be pouring weeks, months or years of your life into building it. Don't let it all go to waste. **Having frequent backups is vital**.
{.is-warning}

Do you care about your health ? Would you take a gamble with your life and forfeit your health insurance ? If your answer is no, then keep reading.

Just like health issues, computer glitches can happen at any time. It is precisely because we cannot anticipate these events, that we take measures to mitigate their potential damage.

> *Still not convinced* ? [Read testimonies](#testimonies) of SuperMemo users who remained skeptic, until it was too late.
{.is-info}

## Proposed strategy

The strategy that we suggest attempts to strike a **balance between robustness and ease of use**. This is not a foolproof method, but it should be robust enough that you do not lose more than a single session of SuperMemo.

> It shouldn't take you more than **a few seconds** to commit your hard work to **safety**.

In this guide, you are going to implement two layers of safety:
1. *Local backups*: Frequent (15 minutes), cheap (disk size), without interruption (you can use SuperMemo concurrently).
2. *Internet backups*: On-demand (after every session), long-term storage (unlimited).

As of the moment of writing this guide (2020/02), this solution is **free** (as in free beer, and in freedom). As an added bonus, you will also be able to **synchronize your collection** between computers.

# Step-by-step guide

## Local backups: BitShelter

[BitShelter](https://github.com/alexis-/BitShelter) *(a.k.a. SuperMemo Backup)* is a software that keeps a version history of your files. It is similar to the Ctrl+Z feature of text editors, only for files.

### I) (*Optional*) Create a partition for your SuperMemo collections

For easier management of your files, and to save space for the frequent snapshots (more on this later), we recommend creating a partition dedicated to your SuperMemo collection. A partition will allow you to keep your SuperMemo files completely seperated from your Window's C:/ drive. 

> If you do not know how to create a partition in Windows, you can [follow this guide](https://www.tomshardware.com/news/how-to-make-partitions-windows-10,36643.html).
{.is-info}

You should obtain a layout similar to this one (it is fine if you only have one disk, instead of two as in this example):

![](/reference-manual/backup-guide/computer-management-disks.png 'SuperMemo partition')


### II) Install & Configuration

#### Installing BitShelter

> Note that BitShelter won't run on 32 bit systems.
{.is-info}

1. Download and install [the latest version](https://github.com/alexis-/BitShelter/releases) of *BitShelter*
2. Start **BitShelter Agent** from the Windows Start menu.
3. Double-click on the [Tray Icon](/reference-manual/backup-guide/bitshelter.agent_trayicon.png) 🖼️

#### Enabling Windows' Volume Snapshot Service (VSS)

> Take note of the Drive Letter which contains your SuperMemo collection. If you only have one disk in your computer, it should be C:\\
> 
> **In this example, the SuperMemo collection Drive Letter is E:\.**
{.is-info}

1. In the [Main Window](/reference-manual/backup-guide/bitshelter.agent_rules.png), click on the <kbd>**Add Schedule**</kbd> button.

> If BitShelter displays [an error](/reference-manual/backup-guide/bitshelter-error.png) about loading AlphaVSS.x64.dll, install vc_redist.x64.exe from [this link](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads).
{.is-info}

2. Click on <kbd>**Enable other Drive(s)**</kbd> in the [General tab](/reference-manual/backup-guide/bitshelter.agent_general.png)
3. Select the SuperMemo drive **(E:\\)** in the [System Protection dialog](/reference-manual/backup-guide/systempropertiesprotection_2018-05-05_13-10-18.png) and click on <kbd>**Configure**</kbd>.
4. In the [new dialog](/reference-manual/backup-guide/systempropertiesprotection_2018-05-05_13-10-22.png) click on <kbd>**Turn on protection**</kbd>, select at least 2GB of desired reserved space for Snapshots, then press <kbd>**OK**</kbd> to both System Protection and System Properties windows.

> If you chose not to create a dedicated partition for SuperMemo, **increase reserve space significantly**. As BitShelter will then run across your entire C:/ drive, it will be filled by all modifications made by any files in windows rather than SuperMemo alone.
{.is-warning}

5. Back in the [General tab](/reference-manual/backup-guide/bitshelter.agent_general.png), click on <kbd>**Raise limit**</kbd>, and set the new limit to **512**.


#### Creating snapshot rules in BitShelter

1. Frequent snapshots (15 min)
    1. Click on the <kbd>**Add Schedule**</kbd> button
        - Select the SuperMemo **Drive letter (E:\\)**
        - Set **Lifetime** to *1 Day*
    2. Click on the <kbd>**Schedule**</kbd> **tab** and fill in [the following values](/reference-manual/backup-guide/bitshelter-15min-schedule.png)
        - **Occurs every**: *15 minutes*
	      - **Frequency**: *Daily*
	      - **Recurs every**: *1 day(s)*
	      - **End on**: *Never*
    3. Press the **Create** button
2. Daily snapshots
    1. Click on the <kbd>**Add Schedule**</kbd> button
        - Select the SuperMemo **Drive letter (E:\\)**
        - Set **Lifetime** to *6 Month*
    2. Click on the <kbd>**Schedule**</kbd> **tab** and fill in [the following values](/reference-manual/backup-guide/bitshelter-daily-schedule.png)
        - **Occurs once at**: *08::00::00 (or whenever your computer is running)*
        - **Frequency**: *Daily*
        - **Recurs every**: *1 day(s)*
        - **End on**: *Never*
    3. Press the **Create** button

Your final BitShelter settings should look similar to the following configuration:

![](/reference-manual/backup-guide/bitshelter-rules.png)

### You are done... Almost !

> It is highly recommended that you **make sure everything is working as intended**.
{.is-info}

Try out the following instructions and see if you're actually able to open up and use a copy made by BitShelter.

#### Oh no. Something happened to my Collection. How to save the day ?

Don't panic! Restoring your collection to an earlier version is easy with BitShelter! 

1. Right click on your collection folder and click on **Restore previous versions**

![](/reference-manual/backup-guide/bitshelter-restorepre.png)

2. Click on the copy you'd like to go back to:

![](/reference-manual/backup-guide/bitshelter-restoremenu.png)

3. You can then click restore, to overwrite current version of the folder, or click open to browse the files:

![](/reference-manual/backup-guide/bitshelter-restoremenu2.png)

> If you have issues with the above instuctions, you can also refer to [this guide](https://www.howtogeek.com/howto/11130/restore-previous-versions-of-files-in-every-edition-of-windows-7/)
{.is-info}

## Internet backups: Git & Github

### Git 101

> **Git** is a tool that makes it easier to track changes to files. When you edit a file, git can help you determine exactly *what* changed, *who* changed it, and *why*. <br /><br />It is useful for coordinating work among multiple people on a project, and for tracking progress over time by saving “checkpoints”. You could use it while writing an essay, or to track changes to artwork and design files. [\[1\]](https://hackernoon.com/understanding-git-fcffd87c15a3)
{.is-info}

**For our purposes**, ***git*** will be our mean to:
- Create versions of our collection (*\"checkpoints\"*).
- Upload\* our work to a safe\*\*, remote place.
- *(Bonus)* Synchronize our work between devices.

\*: GitHub has a 1GB limit on free private repositories. [GitLab](https://about.gitlab.com) offers 10gb free storage by default and [BitBucket](http://bitbucket.org) offers a 5gb plan for 3$. 

\*\*: *Although GitHub can be considered fairly reliable, we highly recommend that you implement a solution to encrypt your collection. This is, after all, a way to your innermost thoughts.*

### Installing & Setting up Git with GitHub

> If you want to use SSH authentication instead of HTTPS, follow [this guide](https://vladmihalcea.com/tutorials/git/windows-git-ssh-authentication-to-github/)
{.is-info}

1. Create a [GitHub account](https://github.com/join/).
2. Download [Git for Windows](https://gitforwindows.org/).
3. Install it with default settings
5. Open a command prompt: type `cmd.exe`, then press <kbd>Enter</kbd> and run the following two commands (with your own name and email you use for github):

```bash
git config --global user.name "Alexis Incogito"
git config --global user.email alexis@incogito.org
```
   
Setup is now complete!
  
### Creating & Synchronizing your GitHub repository

In this example, the GitHub repository we create will be named **SuperMemo-Collection**.

1. Create a [new repository](https://github.com/new):
    - Give a name to your new repo (e.g. *SuperMemo-Collection*)
    - Select **Private**

![](/reference-manual/backup-guide/gitsetup-initialize.png)

2. In your SuperMemo Drive (**E:\\**), open a command prompt: type `cmd.exe`, then press <kbd>Enter</kbd>

![](/reference-manual/backup-guide/windows-explorer-cmd.png)

3. Go to your **GitHub repository** web page, click the <kbd>**Clone or download**</kbd> button, and **press use HTTPS**.

![](/reference-manual/backup-guide/github-clone-link.png)

4. Copy the link starting with `https://`

![](/reference-manual/backup-guide/gitsetup-clonehttps.png)

5. In the **command prompt**, type `git clone <https://github.com/......>`. Replace the text between **< >** with the link you copied from GitHub. 'git clone' will create a local copy of your github repository. 

6. A popup will appear. Login with your GitHub account to authenticate.

![](/reference-manual/backup-guide/gitsetup-login.png)

7. Your repository is now synchronized with your computer. Copy your SuperMemo collection into the new folder. Your folder should look similar to the example below (*.gitignore* might be missing):

![](/reference-manual/backup-guide/git-local-collection-repository.png)

8. <a href="/reference-manual/backup-guide/sm-main-commit.bat" target="_blank" rel="noopener">Download this .bat file</a> and save it in your local repository folder (where your `.git` directory is located). It contains the following commands:

```bash
git add -A && git commit -m "Update"
git push
```

9. Run `sm-main-commit.bat` (double click). If all went well, your should be able to see your collection in your GitHub repository web page.

### Pushing (*\"saving\"*) your work to GitHub

> Every time you finish using SuperMemo, make sure to run `sm-main-commit.bat`.
{.is-info}

That's all ! Your collection is synchronized online, congratulations !

### Optional: Pin commit script to taskbar

To make running sm-main-commit.bat more convenient, you can add it to taskbar. Windows doesn't let you add .bat files to taskbar so instead you can do the following:

1. Right click on sm-main-commit.bat and click [create shortcut](/reference-manual/backup-guide/shortcut-creation.png).

2. The new shortcut still can't be added to taskbar. As such, right click properties and [go to shortcuts menu](/reference-manual/backup-guide/shortcut-edit.png). Add ```cmd /c``` (```cmd \c``` will not work) to the front of [the target script](/reference-manual/backup-guide/shortcut-target.png) and press apply.

3. You can now [right click the shortcut](/reference-manual/backup-guide/shortcut-taskbar.png) and add it to taskbar. After you are done using SuperMemo, click the shortcut in taskbar (or use winkey + taskbar position number key) to sync changes to your collections's Github repository.nt files that haven't been uploaded before running sm-main-pull.bat as it will overrite all local changes

# Why not use Dropbox or Google Drive for backups?

A common question people ask is "**Why not use Dropbox or Google Drive for backups?**".

Admittedly, these are much more user friendly and require very little set up. However, there are a number of reasons why these services are inadequate for our purposes.

1. It is very easy to get something wrong, and corrupt your collection due to file locks. Previous backup methods relied on watching and killing processes in an effort to prevent this, but these are very inelegant solutions.

2. Syncing to a cloud provider pushes each file individually without any knowledge of how they are grouped together. If for some reason your cloud provider messes up the syncing, it might lead to nasty results. By contrast, the git push to server is an atomic transaction, meaning it either completely succeeds, or completely fails, there is no situation where your collection data gets partially backed up.

# Suggestions to improve your backup strategy

> Work in progress. Come back later !

- [Encrypt your GitHub repository](https://github.com/AGWA/git-crypt).
- Implement the [3-2-1 Backup Rule](https://www.acronyms-it.co.uk/blog/backup-rule-of-three/) [(Visual Guide)](/reference-manual/backup-guide/321backup.png){target="_blank"}.
- Make your SuperMemo partition a [Mirrored Volume (RAID 1)](https://www.windowscentral.com/how-set-mirrored-volume-file-redundancy-windows-10).

# Testimonies

> 💬 **Luke Avedon**: “*Back up your collection.  I'm ashamed to admit I used to never back up my collection.  Once while running a quick, 'repair collection' I lost power.  An entire section of my knowledge tree was mangled forever.  All the references changed to strange, incomprehensible characters.  Now I know better.  I automatically back up to two local hard drives, and three cloud drives each day.*”

> 💬 **Nour**: “*Well, I'm a bit new to SM and although I was warned, I did not understand the gravity of the warnings. Back-up your collection. Since I'm new, I don't understand a lot of the issues, but I know I didn't do anything to provoke them, and yet the combination of SM and my virtual machine had corrupted and misplaced files and needed to be repaired – with the repairs yielding some unwanted adjustments to my collection. Of course, if all your final prep is on SM, you'd be having heart palpitations at the thought of your collection getting messed up, I know I was. Sufficed to say lesson learned. The hard way, but learned never-the-less.*”

> 💬 **Supersrdjan**: “*I used supermemo for two years enjoying steady gains as my collection grew. I backed up my collection daily at first. But it seemed like overkill. So I switched to weekly backups. Sometimes I would skip a week, or two, and then weeks turned into months between backups. Of course, one day, inevitably, Supermemo crashed and wiped my collection. I felt worse than a stockbroker in 1929. I was about to fall into a great depression.  I had to revert to a 3-month old backup. Better than total bankruptcy I guess. But those months aren't coming back.*”
