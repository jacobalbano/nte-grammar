# nte-grammar
A progressive grammar guide for Japanese, collaboratively developed by the 日本語と英語 discord server.

An [Obsidian](https://obsidian.md/) vault.

Outline and guidelines coming soon.

# Setup
For experienced git users: 
- Clone this repository into the folder of your choice
- Open the folder as a vault in Obsidian

For beginners to git:
- Install git from the instructions [here](https://github.com/gitobsidiantutorial/obsidian-git-tut-windows/blob/main/README.md#software-installation)
	- Make sure to also follow the section about installing [Github Desktop](https://desktop.github.com/) and logging in
- Download this repository as a zip archive from the green "Code" button → Download Zip
- Unpack the archive into a directory of your choice
	- (Windows): run `initialize_git.bat`
	- (Mac/Linux): run `initialize_bat.sh`
- Open the folder as a vault in Obsidian

The first time you open the vault, you'll be prompted to trust plugins. The only plugins currently in use are:
- [Obsidian-git](https://github.com/denolehov/obsidian-git)

Trusting plugins is not essential but you will have to manage sync manually, and other features may not work in the future.

# Sync
The obsidian vault in this repository includes a plugin which hides a lot of the nitty-gritty details of git.

Open the sync sidebar by opening the command pallette (**ctrl+p**) and typing "open source control view".

"Staged Changes" are files which you want included in the sync.

"Changes" are files which have not yet been staged. Click the + button on each item to manually stage it. You can also click the "Stage All" button at the top to add all files immediately.

"Commit" marks all staged files as being part of a group of files you want to upload.

"Pull" downloads changes from the server; "Push" uploads your committed files.