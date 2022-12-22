---
title: Backup Strategy Guide
description: Learn how to protect your months or years of investment. Set it up once, and forget about it!
published: true
date: 2022-12-22T12:58:17.291Z
tags: 
editor: markdown
dateCreated: 2020-12-06T14:16:06.567Z
---

# Why & How?

## Why should you backup?

> ⚠️ **Your collection is precious**. If you are using SuperMemo, you will likely be pouring weeks, months or years of your life into building it. Don't let it all go to waste. **Having frequent backups is vital**.
{.is-warning}

Do you care about your health? Would you take a gamble with your life and forfeit your health insurance? If your answer is no, then keep reading.

Just like health issues, computer glitches can happen at any time. It is precisely because we cannot anticipate these events, that we take measures to mitigate their potential damage. This is what we propose to do in this guide.

> *Still not convinced?* [Read testimonies](#testimonies) of SuperMemo users who remained skeptic, until it was too late.
{.is-info}

## Proposed strategy

The strategy we suggest attempts to strike a **balance between robustness and ease of use**. This is not a foolproof method, but it should be robust enough that you do not lose more than a single study session at any time.

> It shouldn't take you more than **a few seconds** to commit your hard work to **safety**.

In this guide, you are going to implement two layers of protection:
1. *Local backups*: Frequent (15 minutes), cheap (disk size), without interruption (you can use SuperMemo concurrently).
2. *Internet backups*: On-demand (after every session), long-term storage (unlimited).

As of the moment of writing this guide (2020/02), this solution is **free** (as in free beer, and in freedom). As an added bonus, you will also be able to **synchronize your collection** between computers.

# Step-by-step guide

## Local backups: BitShelter

[BitShelter](https://github.com/alexis-/BitShelter) *(a.k.a. SuperMemo Backup)* is a software that keeps a version history of your files. It is similar in concept to using Ctrl+Z in your favourite text editor, only applied to files.

### I) Create a partition for your SuperMemo collections

A partition keeps your SuperMemo files completely seperate from your Window's C:/ drive, with the following benefits:
- Fully dedicates the snapshot disk space to SuperMemo ;
- Better organization and easier management of your precious files.

**Not creating a partition for your SM collection puts you at risk**. _Explanation_:
> Imagine that you have been conscientiously using SuperMemo with the peace of mind that your work is backed up and secure.
> 
> You've worked hard today and want to indulge in watching a movie. You watch the movie, it was good, and now that it's finished, you delete the 5GB file (it's HD).
> 
> Now you go back to your collection and realize that you have mistakenly deleted a whole branch. You look into your backup history, but to your horror it is empty!
>
> In fact, deleting that 5GB file filled your snapshot reserve space with the movie's content. And since your snapshot reserve size was 5GB, it filled the entire space, flushing out previous data from your collection.

Creating a partition will dedicate the entire snapshot reserve space to content on that partition only. It will help to prevent a story like that from happening to you.

#### Partition size

Determining the correct partition size depends on a few factors, including:
- Available free space on your disk,
- Volume of media material (PDF, videos, audio, ...) you will import in your collection,
- Margin of error you are willing to leave yourself.

Avoid partition sizes lower than 8GB. If you reserve 3GB for saving your file history, only 5GB of free space will be left available for you to use on the partition.

> It is **imperative** that you never use more than the file space available on the partition. In our example earlier, you must never use more than 5GB of space for your files.
>
> Not following this principle will result in **corrupting your files**. The same principle applies even if you do not create a dedicated partition (e.g. if you use C:\).
{.is-warning}

#### Creating the partition

- [<span style="color: #666;" class="mdi mdi-harddisk-plus mr-1"></span> Creating a Windows partition *Toms Hardware guide.*](https://www.tomshardware.com/news/how-to-make-partitions-windows-10,36643.html)
{.links-list}

You should obtain a layout similar to this one (it is fine if you only have one disk, instead of two as in this example):

![](/reference-manual/backup-guide/computer-management-disks.png 'SuperMemo partition')

### II) Installation & Configuration

#### Installing BitShelter

> Note that BitShelter won't run on 32 bit systems.
{.is-info}

1. Download and install [the latest version](https://github.com/alexis-/BitShelter/releases) of *BitShelter*
2. Start **BitShelter Agent** from the Windows Start menu.
3. Double-click on the [Tray Icon](/reference-manual/backup-guide/bitshelter.agent_trayicon.png).

#### Enabling Windows' Volume Snapshot Service (VSS)

> Take note of the Drive Letter which contains your SuperMemo collection. If you only have one disk in your computer, it should be C:\\
> 
> **In this example, the SuperMemo collection Drive Letter is E:\\.**
{.is-info}

1. In the [Main Window](/reference-manual/backup-guide/bitshelter.agent_rules.png), click on the <kbd>**Add Schedule**</kbd> button.

> If BitShelter displays [an error](/reference-manual/backup-guide/bitshelter-error.png) about loading AlphaVSS.x64.dll, install vc_redist.x64.exe from [this link](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads).
{.is-info}

2. Click on <kbd>**Enable other Drive(s)**</kbd> in the [General tab](/reference-manual/backup-guide/bitshelter.agent_general.png).
3. Select the SuperMemo drive **(E:\\)** in the [System Protection dialog](/reference-manual/backup-guide/systempropertiesprotection_2018-05-05_13-10-18.png) and click on <kbd>**Configure**</kbd>.
4. In the [new dialog](/reference-manual/backup-guide/systempropertiesprotection_2018-05-05_13-10-22.png) click on <kbd>**Turn on protection**</kbd>, select at least 2GB of desired reserved space for Snapshots, then press <kbd>**OK**</kbd> to both System Protection and System Properties windows.

> If you chose not to create a dedicated partition for SuperMemo, **increase reserve space significantly**. All changes on your drive (e.g. C:\\) will be tracked and counted towards the file history space.
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

### You are done... Almost!

> It is highly recommended that you **make sure everything is working as intended**.
{.is-info}

Try out the following instructions and see if you're actually able to open up and use a copy made by BitShelter.

#### Oh no. Something happened to my Collection. How to save the day?

Don't panic! Restoring your collection to an earlier version is easy with BitShelter! 

1. Right click on your collection folder and click on **Restore previous versions**

![](/reference-manual/backup-guide/bitshelter-restorepre.png){.ml-8}

2. Click on the copy you'd like to go back to:

![](/reference-manual/backup-guide/bitshelter-restoremenu.png){.ml-8}

3. You can then click restore, to overwrite current version of the folder, or click open to browse the files:

![](/reference-manual/backup-guide/bitshelter-restoremenu2.png){.ml-8}

> If you have issues with the above instructions, you can also refer to [this guide](https://www.howtogeek.com/howto/11130/restore-previous-versions-of-files-in-every-edition-of-windows-7/)
{.is-info}

## Internet backups: Git

### Git 101

> **Git** is a tool that makes it easier to track changes to files. When you edit a file, git can help you determine exactly *what* changed, *who* changed it, and *why*. <br /><br />It is useful for coordinating work among multiple people on a project, and for tracking progress over time by saving “checkpoints”. You could use it while writing an essay, or to track changes to artwork and design files. [\[1\]](https://hackernoon.com/understanding-git-fcffd87c15a3)
{.is-info}

**For our purposes**, ***git*** will be our means to:
- Create versions of our collection (*\"checkpoints\"*).
- Upload^1^ our work to a safe^2^, remote place.
- *(Bonus)* Synchronize our work between devices.

---
^1^: At this date (2020/02), [GitLab](https://about.gitlab.com) offers 10gb of free storage. GitHub offers 1GB of free storage for private repositories. [BitBucket](http://bitbucket.org) offers a 5gb plan for 3$.

^2^: Although the listed Git providers can be considered fairly reliable from a technical standpoint, we highly recommend that you implement a solution to encrypt your collection. Your collection is a map to your brain and to your innermost thoughts. Don't let others peer into it without your consent.

### Installing & Setting up Git

> If you want to use SSH authentication instead of HTTPS, follow [this guide](https://vladmihalcea.com/tutorials/git/windows-git-ssh-authentication-to-github/)
{.is-info}

1. Download [Git for Windows](https://gitforwindows.org/).
2. Install it with default settings
3. Open a command prompt: type `cmd.exe`, then press <kbd>Enter</kbd> and run the following two commands (with your own name and email you use for github):

```bash
git config --global user.name "Alexis Incogito"
git config --global user.email alexis@incogito.org
```
   
Setup is now complete!
  
### Creating your repository

In this example, the repository we create will be named **SuperMemo_Collection**.

You can choose from a variety of providers. We recommend using GitLab, because:
1. The free plan offers more file space than its alternatives,
2. It tracks the history of large files, which is important for collection with large text registries,
3. GitHub is owned by Microsoft, a company infamous for its poor privacy policy.

#### GitLab

- [1. Create a new account *Register on GitLab.*](https://gitlab.com/users/sign_up){target="_blank"}
- [2. Create a new repository *New GitLab project.*](https://gitlab.com/projects/new#blank_project){target="_blank"}
{.links-list}

**🚧 Work in progress.**

#### GitHub

- [1. Create a new account *Register on GitHub.*](https://github.com/join/){target="_blank"}
- [2. Create a new repository *New GitHub repository.*](https://github.com/new){target="_blank"}
{.links-list}

Input the following information in your new repository:
- Give a name to your new repo (e.g. *SuperMemo_Collection*)
- Select **Private**

![](/reference-manual/backup-guide/gitsetup-initialize.png){.ml-8}

### Synchronizing your Git repository

#### Existing collections

To use git **with an existing collection**:

1. Rename the folder containing your collection,
2. Follow the instructions below,
3. Move all your collection files into the directory created with `git clone`.

#### Cloning the repository

1. Press <kbd class="win"></kbd> + <kbd>E</kbd> to **open Windows Explorer**,
2. **Navigate to your SuperMemo drive**, in our example, drive **`E:\`**,

![windows-explorer-drives.png](/reference-manual/backup-guide/windows-explorer-drives.png){.ml-8}

3. **Open a command prompt**:
    1. Click on the bar at the top where it read `E:\`,
    2. Type `cmd.exe`, then press <kbd>Enter</kbd>.
    ![](/reference-manual/backup-guide/windows-explorer-cmd.png){.ml-8}

4. In your browser, navigate to your **repository web page**, and copy the *git url*:
    - _GitLab_: Click the <kbd>**Clone**</kbd> button, then copy the link under **Clone with HTTPS**,
    ![gitlab-clone-link.png](/reference-manual/backup-guide/gitlab-clone-link.png){.ml-8}
    - _GitHub_: Click the <kbd>**Clone or download**</kbd> button, press <kbd>Use HTTPS</kbd>, then **copy the link**.
    ![](/reference-manual/backup-guide/github-clone-link.png){.ml-8}
    ![](/reference-manual/backup-guide/gitsetup-clonehttps.png){.ml-8}

5. In the **command prompt**, type `git clone <https://gitlab.com/......>`.

Replace the text between **< >** with the link copied previously. `git clone` will create a local version of your Git repository.

6. **Login** with your account. A popup will appear:
    - _GitLab_:
    **🚧 Work in progress.**{.ml-8}
    - _GitHub_:
    ![](/reference-manual/backup-guide/gitsetup-login.png){.ml-8}

7. Your repository is now synchronized with your computer and **a new folder** has been created.

**Copy your SuperMemo collection** into the new folder. In our example it will be located in `E:\SuperMemo_Collection\`.{.ml-8}

Your folder should look similar to the example below (*.gitignore* might be missing):{.ml-8}

![](/reference-manual/backup-guide/git-local-collection-repository.png){.ml-8}

#### Pushing (*\"saving\"*) your work to git

> Every time you finish using SuperMemo, **make sure to synchronize your collection** using of the methods below.
{.is-info}

##### Simple synchronization

1. <a href="/reference-manual/backup-guide/sm-main-commit.bat" target="_blank" rel="noopener">Download this .bat file</a> and save it in your local repository folder (where your `.git` directory is located). It contains the following commands:

```bash
git add -A && git commit -m "Update"
git push
```

2. Run `sm-main-commit.bat` (double click). If all went well, your should be able to see your collection in your GitHub repository web page.

That's all! Your collection is synchronized online, congratulations!

##### Advanced synchronization

Community member **@Owl** created an advanced synchronization scripts with the following benefits:

1. Facilitates synchronizing collections across computers with git ;
2. Provides additional safety by further automating pushing to git, and protecting you against forgetfullness ;

- [📥 &nbsp; Download and Install *SuperMemo-Git-sync*](https://github.com/supermemo/SuperMemoScripts/tree/master/SuperMemo-Git-sync)
{.links-list}

### Optional: Pin commit script to taskbar

To make running sm-main-commit.bat more convenient, you can add it to taskbar. Windows doesn't let you add .bat files to taskbar so instead you can do the following:

1. Right click on sm-main-commit.bat and click [create shortcut](/reference-manual/backup-guide/shortcut-creation.png).

2. Edit the new shortcut to make it pinnable in the taskbar:
    1. Right-click <kbd>Properties</kbd> and [go to shortcuts menu](/reference-manual/backup-guide/shortcut-edit.png)
    2. Add ```cmd /c``` to the front of [the target script](/reference-manual/backup-guide/shortcut-target.png)
    3. Click on <kbd>Apply</kbd>.

3. Right-click the shortcut and [add it to taskbar](/reference-manual/backup-guide/shortcut-taskbar.png).

Every time you are done using SuperMemo, click on the shortcut in the taskbar to sync changes to your collections's Github repository.

> You can also use this keyboard shortcut to quickly execute the script: <kbd class="win"></kbd> + <kbd>number key</kbd>.
> 
> *Number key* is the position of the script in your taskbar (e.g. <kbd>1</kbd> <kbd>2</kbd> ...).
{.is-info}

# Why not use Dropbox or Google Drive for backups?

A common question people ask is "**Why not use Dropbox or Google Drive for backups?**".

Admittedly, these are much more user friendly and require very little set up. However, there are a number of reasons why these services are inadequate for our purposes.

1. It is very easy to get something wrong, and corrupt your collection due to file locks. Previous backup methods relied on watching and killing processes in an effort to prevent this, but these are very inelegant solutions.

2. Syncing to a cloud provider pushes each file individually without any knowledge of how they are grouped together. If for some reason your cloud provider messes up the syncing, it might lead to nasty results. By contrast, the git push to server is an atomic transaction, meaning it either completely succeeds, or completely fails, there is no situation where your collection data gets partially backed up.

# Suggestions to improve your backup strategy

> Work in progress. Come back later!

- [Encrypt your GitHub repository](https://github.com/AGWA/git-crypt).
- Implement the [3-2-1 Backup Rule](https://www.acronyms-it.co.uk/blog/backup-rule-of-three/) [(Visual Guide)](/reference-manual/backup-guide/321backup.png){target="_blank"}.
- Make your SuperMemo partition a [Mirrored Volume (RAID 1)](https://www.windowscentral.com/how-set-mirrored-volume-file-redundancy-windows-10).

## Duplicati Backup Guide

### Installing Duplicati on Windows

I assume you're on Windows. Go to [Duplicati download page](https://www.duplicati.com/download), click the "Windows 2.0.5.1" icon to download the Windows installer. If you have a 32-bit version Windows, download the Windows 32 bit installer instead.

During installation, no change is needed: just keep pressing Next until complete. After installation, a new Duplicati tray icon in the System Tray will appear. Right click on it-> Click open to open the app:

![icon_1.png](/duplicatibackup/icon_1.png)

It's a browser-based app. Your default browser will open and launch a new tab at http://localhost:8200/ngax/index.html.

### First backup

In this tutorial I'll back up the whole SuperMemo Drive (:S) to Google Drive as an example. The following are my suggested settings. Feel free to modify as you see fit.

In the Duplicati homepage, click "Add backup":

![t05_1.png](/duplicatibackup/t05_1.png)

The default "Configure a new backup" should be selected. Click Next.

#### 1. General

![t1_1.png](/duplicatibackup/t1_1.png)

I __highly recommend__ that you choose Encryption: "AES-256 encryption, built in". Without encryption all your data is exposed.

Passphrase is another term for password. Please make it long and store it to a secure location. If you lose this passphrase you won't be able to decrypt your precious precious collection when needed.

Click Next

#### 2. Backup destination

![t2_1.png](/duplicatibackup/t2_1.png)

"Path on server" means the folder name in your Google Drive. Don't worry if it doesn't exist yet. Duplicati will create it for you later.

Click the blue AuthID link. Choose your login credentials. After authentication a string will appear in the input field.

Click Test connection. It'll prompt "The folder SuperMemoBackup does not exist. Create it now?" Click yes.

Click Next

#### 3. Source data

![t3_1.png](/duplicatibackup/t3_1.png)

I've followed the above "Local backups: BitShelter" guide, so I choose the whole drive as source data.

#### 4. Schedule

![t4_1.png](/duplicatibackup/t4_1.png)

I choose to back up every 3 hours. Feel free to change it.

#### 5. Options

Keep the default. Click Save

After this, go back to the homepage and you'll see a new task has appeared. Click Run. After that Duplicati will run your task automatically.

![t5_1.png](/duplicatibackup/t5_1.png)

For more please read [Duplicati 2 User's Manual](https://docs.duplicati.com).

# Testimonies

> 💬 **Supersrdjan**: “*I used supermemo for two years enjoying steady gains as my collection grew. I backed up my collection daily at first. But it seemed like overkill. So I switched to weekly backups. Sometimes I would skip a week, or two, and then weeks turned into months between backups. Of course, one day, inevitably, Supermemo crashed and wiped my collection. I felt worse than a stockbroker in 1929. I was about to fall into a great depression.  I had to revert to a 3-month old backup. Better than total bankruptcy I guess. But those months aren't coming back.*”

> 💬 **Luke Avedon**: “*Back up your collection.  I'm ashamed to admit I used to never back up my collection.  Once while running a quick, 'repair collection' I lost power.  An entire section of my knowledge tree was mangled forever.  All the references changed to strange, incomprehensible characters.  Now I know better.  I automatically back up to two local hard drives, and three cloud drives each day.*”

> 💬 **Nour**: “*Well, I'm a bit new to SM and although I was warned, I did not understand the gravity of the warnings. Back-up your collection. Since I'm new, I don't understand a lot of the issues, but I know I didn't do anything to provoke them, and yet the combination of SM and my virtual machine had corrupted and misplaced files and needed to be repaired – with the repairs yielding some unwanted adjustments to my collection. Of course, if all your final prep is on SM, you'd be having heart palpitations at the thought of your collection getting messed up, I know I was. Sufficed to say lesson learned. The hard way, but learned never-the-less.*”

> 💬 **Godfreyla**: "*I had an issue with my hard drive, and to cut a long story short my laptop died. I had around 2 years’ worth of Supermemo use completely gone! But fortunately, I’d followed the guidance around setting up local backups and more importantly, internet backups using git and GitLab. It might take you a couple of hours to set up (and in the process you learn some new things), but knowing what I do now, I’d go so far to say it’s probably not worth the risk of using SM without having this backup strategy in place!*"