---
layout: post
title:  "Zotero Sync Folder"
date:   2019-03-11 12:38:58 +0100
categories: tutorial update
---

![header](assets/viktor-talashuk-05HLFQu8bFw-unsplash.jpg)

Photo by [Viktor Talashuk](https://unsplash.com/@viktortalashuk?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on Unsplash.

## Why Zotero?

Zotero is a great tool and performs very well as a citation manager. It has the classic features like Word and OpenOffice integration and some more unique ones such as google Docs integration (at writing time, only paperpile has a decent support for this). Also, it’s the open source ([AGPL](https://en.wikipedia.org/wiki/Affero_General_Public_License)) solution which has decent features for a quite competitive market ([JabRef](https://www.jabref.org/) is also FOSS but looks ugly IMO). If Zotero is not your thing, [Mendeley](https://www.mendeley.com/?interaction_required=true), [ReadCube](https://www.readcube.com/home) and [Paperpile](https://paperpile.com/) are other options.

One caveat of Zotero is the lack of a mobile app, I am not sure whether it’s a good idea anyway but it’s a feature request that has been around for a while now. (There are some third party apps out there, never tested). This worries me little in general.

The second caveat which I consider more relevant is the lack of storage space in the sync platform. In Zotero Sync the storage limit for the free account is only [300 MB](https://www.zotero.org/storage). Mendeley however, it has 2Gb storage limit which is more decent. Currently my library has 964 MB (for 300ish papers) so Mendeley could still be fine for me.

I don’t like mendeley for various reasons though, main reasons are that the software was IMHO unreliable, the sync time was slow and Mendeley is now part of Elsevier (which might be less relevant to other people). Also a important reason to switch might have been that my previous Mendeley library was a complete mess so I felt like a fresh start would fix a lot of things (spoiler alert, it didn't). I was also not happy in sharing the pay-walled papers to their servers for various reasons.

In order to overcome those problems I found that the best solution (for me) was to independently host my pdf library somewhere safe so I could, in one hand not depend on a “social network” reference manager but at the same time have synced pdfs. 

My current workflow uses Zotero, ZotFile (Add-on) and Google Drive. This is also handy as the files in the google drive are sorted and accessible for example to import in my note-taking application in the iPad.

## Steps to set it up:

This blog post is mostly for self-reference but some people might find it useful. We will need a sync folder which I would refer to as SYNC_PATH. Also when installing in a new computer, just fetch the SYNC_PATH again.

(This is recalled by memory but I should be mostly right)

1. Install Zotero (from here https://www.zotero.org/download/)

2. Go to your cloud resource of choice, (eg google drive, dropbox, ...) and then create a folder (SYNC_PATH).

3. Download ZotFile 
Download the file from their website (http://zotfile.com/), it has `.xpi` extension (careful if you are using firefox).

1. Install it in Zotero:

```
Zotero > Tools > Add-ons > Gear Symbol > Add from File > Select Zotero downloaded file
```

1. Restart Zotero

1. Add linked library to path (ZotFile)
   
```
Tools > ZotFile Preferences > General settings > Custom Location: SYNC_PATH
```

You can further configure ZotFile with naming rules and such but this is not covered so far.

1. Add linked library in Zotero


```
Edit > Preferences > Advanced > Files and Folders >  Linked Attachment Base Directory > Base Directory: SYNC_PATH
```

Now everything should be done and every time you add a pdf to Zotero the program should magically rename the file, extract the metadata and upload it to the synced path.

If you already have a pdf in Zotero and you want to send it to the Sync Path via ZotFile.

```
Right click in the pdf > Manage Attachment > Rename File 
```

This will rename the file according to the metadata and place it in the synced path.

