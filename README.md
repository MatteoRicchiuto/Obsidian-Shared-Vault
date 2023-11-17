# Obsidian-Shared-Vault
This is my obsidian repository that contains all my Uni and Coding related notes 

If you download this repository, you will be able to open it with obsidian. 

The vault already has all the plugins that you need to use it.

---
# Table of content

- [Hot-Keys](#Hot-Keys)
- [Plugins](#Plugins)
- [Work-Flows](#Work-Flows)
  - [Crating New Notes](#Crating-New-Notes)
  - [Workspace Layouts](#Workspace-Layouts)
  - [Folder Organisation and Description](#Folder-Organisation-and-Description)
  - [Managing new notes and files](#Managing-new-notes-and-files)
  - [Tab Switching](#Tab-Switching)   
  - [Theme Customisation](#Theme-Customisation)

---
# Hot-Keys

| Key                                       | Description   |
| ----------------------------------------- | ------------- |
| ```cmd``` + ```s``` | Search in all files |
| ```cmd``` + ```shift``` + ```s``` | Show file explorer |
| ```cmd``` + ```shift``` + ```f``` | Search and replace in current file  |
| ```cmd``` + ```f``` |  Search current file |
| ```cmd``` + ```d``` |  Toggle right side bar |
| ```cmd``` + ```shift``` + ```d``` |  Toggle left side bar |
| ```cmd``` + ```w``` |  Close current tab |
| ```cmd``` + ```p``` |  Open command palette |
| to-do | Navigate back  |
| to-do | Navigate forward |
| ```cmd``` + ```r``` | Load workspace layout |
| ```cmd``` + ```shift``` + ```r``` | Save and load workspace layout |

---
# Plugins

These are all the **Community Plugins** that I use in my actual obsidian configuration

| Key                                       | Description   | Work Flow |
| ----------------------------------------- | ------------- | --------- |
| [Advanced Tables](https://github.com/tgrosinger/advanced-tables-obsidian) | Improved formatting and manipulation to markdown tables in Obsidian |  |
| [Folder Note](https://github.com/xpgo/obsidian-folder-note-plugin) | Add description note to a folder  | [link](#Folder-Description) |
| [Latex Suite](https://github.com/artisticat1/obsidian-latex-suite) | Typesetting LaTeX math as fast as handwriting |  |
| [Local Images](https://github.com/aleksey-rezvov/obsidian-local-images) | finds all links to external images in your notes, downloads and saves images locally and finally adjusts the link in your note to point to the local image files |  |
| [Obsidian Git](https://github.com/denolehov/obsidian-git) | Plugin that allows you to back up your Obsidian vault to a remote Git repository |  |
| [Quick Add](https://github.com/chhoumann/quickadd) | Powerful combination of four tools: templates, captures, macros and multis | [link](#Crating-New-Notes) |
| [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) | Customisation settings for obsidian themes | [link](#Theme-Customization) |
| [Tab Switcher](https://github.com/Vinzent03/tab-switcher) |  | [link](#Tab-Switching)  |

---

# Work-Flows

## Crating New Notes

> All new note, files and media are initially saved in the [[To-Do]] folder, and later can be sorted in the right folders

**Base metods:**

| Key                                       | Description   |
| ----------------------------------------- | ------------- |
| ```cmd``` + ```n``` | Create new note |
| ```cmd``` + ```shift``` + ```n```| Create new note to the right |
| ```cmd``` + ```t``` | Create new note from templates ([quickadd plugin](https://github.com/chhoumann/quickadd))  |

**Advanced method:**
Creating a new note from a not existing but already defined note (using 
[quickadd plugin](https://github.com/chhoumann/quickadd))
1. hi-light the note name  
2. press ```cmd``` + ```t```  
3. Select the template

> [!note] 
> - This method is implemented using the [quickadd plugin](https://github.com/chhoumann/quickadd) , you can **add new templates** going the settings of this plugin
> - You can also **specify the folder where you want to create the note** in always in the plugin settings (example: "uni note" template creates a note in the "uni_archive" folder )

**Example:**

https://github.com/Jaxkeeper/Obsidian-Shared-Vault/assets/116072651/6dc6f184-d32d-4fff-96a3-b0e27a479e5d


---
## Workspace Layouts

> To use this workflow you have to turn on the ```Workspaces plugin``` in the core-plugins settings 

**Create a new workspace layout:**
1. Presa ```cmd``` + ```p``` to open command palette
2. Search ```Workspace: Manage workspaces layouts```
3. Create and save a new workspace layout

**Load an existing layout:**
-  Press ```cmd``` + ```r``` and choose the layout

**Save and load another layout:**

If you have already opened a layout, you can: 
- *Save it:* press ```cmd``` + ```shift``` + ```r```, than choose the layout that you have already opened
- *Save and load a different one:* press ```cmd``` + ```shift``` + ```r```, than choose the layout that you want to open

**Example:**

https://github.com/Jaxkeeper/Obsidian-Shared-Vault/assets/116072651/141ec72f-1982-47b5-8129-8d0247f871b7

---
## Folder Organisation and Description

There are 2 main way to organise you vault:
	- **Tags organisation:** 
		- All notes and files are divided in a small amount of folders, links and tags are used to categorise and organise your notes
		- Pros: Easy to maintain
		- Cons: not modular (it's hard to remove/move a notes categories) it can become disordered if you have lots of notes
	- **Folder organisation:** 
		- All the recurring main topics and subjects have their own folder and usually different types of files are divided in different folders
		- Pros: tidy and ordered, modular
		- Cons: organising all the notes and file is hard and time consuming (not productive)

**How i organise my vault:** I my case i use a combination of these 2 organisation techniques

#### Key Features:
- **Modularity:** I want all my notes to divided in folder by category (example: university notes, Coding and technical notes, Journaling ...). This is important because i can treat them as separated vaults (example: one day i could decide to remove all my university notes from my main vault and make the in a new separate one)
- **Easily maintainable:** Creating new notes and organising them is easy and fast

### Folder Structure
**Index:**
- [Easy Notes folder](#Easy-Notes-folder)
- [Literature Notes folder](#Literature-Notes-folder)
- [Mocs folder](#Mocs-folder)
- [Storage folder](#Storage-folder)
- [To-Do folder](#To-Do-folder)

<img src="README_media/" width="600">

**add image**

####Easy Notes folder  
This folder has **no rules**, i usually save here:
- *Small notes* that i don’t know where to save 
- Random *thoughts and Ideas*

### Literature Notes folder
This folder has only one rule, the notes need to be long and well written. I usually save here:
- Long and articulated notes that i don’t know where to save
- Books/Films/Games summaries 
- Elaborations of the notes that are in the "Easy Notes" folder

### Mocs folder
This is my main and most important folder
It contains other folders (subfolders), every subfolder as is own topic.

>I have here only groups of notes that i want to treat as separated vaults. 

Every subfolder as a precise structure:
```
sub_folder
	- sub_moc.md
	- sub_foler_archive
	- sub_folder_storage
```

- *sub_moc.md:* a map of content (index) where you can link notes related the the main topic of the folder
- *sub_folder_archive:* folder where you can save all the notes related to the topic
- *sub_folder_storage:* folder where you can save all the files related to the topic (example: images, pdfs, ...)

***add image of sub folder***

### Storage folder

This is a general folder where i store all the files, media and templates of the vault that don't fit in the categories of the [[#MOCS folder]] (aggiusta link) 

### To-Do folder

This folder it’s set as default location where all the file, notes and media are saved when imported or created (with out using [[link della tecnica]] ) in the vault.

**Read:** [Managing new notes](#Managing-new-notes) for more information

---



## Managing new notes and files
#### New Notes:
As seen in [Crating New Notes](#Crating-New-Notes) all the notes created with the ```cmd``` + ```t``` hot-key are already created in the right folder so you have to manage them

If you create a note without using the ```cmd```+ ```t``` method or you have crated a random note that doesn’t fit any of your template, it will be saved in the **To-Do Folder**

#### New Files:
All new files when imported in the vault are saved in the **To-do folder**

When you have some spare time you can open this folder and move all the files in the right folders (example: if you have a university related image you can move it to the "uni_storage" folder)

---
## Tab Switching

---
## Theme Customisation

---





