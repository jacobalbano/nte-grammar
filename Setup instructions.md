# Git usage and workflow
This is a step-by-step guide to setting up a way to contribute for people who are not very familiar with git. Some of this stuff is pretty complicated; if something isn't clear feel free to ask.

### Initial setup
- Make a Github account. (If you are on github, there should be a signup button up there)
- Install git on your local computer
	- Go to https://git-scm.com/downloads and choose your OS for a download link.
	- Instal [Github Desktop](https://desktop.github.com). This isn't strictly necessary but is gonna help with later steps. Once you install it, open it so you can log in.
- Install [Obsidian](https://obsidian.md) if you haven't already.
	- You can technically edit these files with any text editor, but this repository is intended to be used with Obsidian.
	- Obsidian is a pretty deep application with lots of cool features. If you're interested or confused you can try looking at the official [Obsidian documentation](https://help.obsidian.md/Obsidian/Index)
- Create a fork.
	- A fork is a copy of this repository, but associated with your account, which means you can do anything you want to it.
	- On the github page, if you're logged in, there should be a button up near the top. ![[git_instructions_a.png]]
	- This button will take you to a new page, you can just click on the green "Create fork" button at the end.
- Now we download the repository. There are other ways of doing it but here's what I recommend for simplicity.
	- On Github Desktop, you should be able to see your fork on a list of your repositories. 
	  ![[git_instructions_b.png]]
	- Click the "Clone {your username}/nte-grammar" button down below.
	- This opens up a dialog where you can change a few things, such as where the folder will go, if you prefer. Then click the blue button to move on.
	- Next you should see this pop up. Make sure to keep "contribute to the parent project" before clicking Continue.
	  ![[git_instructions_c.png]]
- Open up Obsidian.
	- Click "Open" and choose the same folder you set up with Github Desktop. ![[git_instructions_d.png]]
	- The first time you open the vault Obsidian will ask you to trust plugins. This is not mandatory but will help automate some of the tasks involved in syncing. 
		- Currently we have these plugins associated with the vault:
			- [Obsidian-git](https://github.com/denolehov/obsidian-git)

Now you have a full local copy and can make changes as you please. 

### Submitting changes
Your local changes aren't automatically uploaded either to your local fork or submitted to the parent repository. Here's how to do that using the installed obsidian-git plugin. Certain parts here can be automated through plugin settings. Note also that most of the stuff we're using obsidian-git for here can be done through Github Desktop, if you find that interface more approachable.

After you have some changes, open the command palette (pressing **Ctrl-P**, or **Cmd-P** on Mac and type "source control view," then press Enter. A panel like this should open to the right. 
  ![[git_instructions_e.png]]
The buttons on the source control panel are the main controls for interacting with the repositiory. They include some git lingo, so here's a run-down of the lingo and what some buttons do.
- **Staged Changes**: These are the files you want to include in the sync.
- **Changes**: The files which you've changed which have not been staged yet.
	- Each file has a **+** button to the right of its name which you can click to stage that specific file. This means you have control over which files you want to submit and which you're still working on.
- **Commit** (the ✔ button up top): This creates a "snapshot" of all your staged changes so they can be uploaded.
- **Stage All** (the circled **+** up top): This stages everything. So all files in "changes" move to "staged changes".
- **Unstaged changes** (the circled **-** up top): A way to say "oh no go back" and move everything back down to "Changes." This is useful if you accidentally stage everything but would rather do just one or two files instead.
- **Push** (the ↑ button up top): Uploads _committed_ changes to your fork. This means that things in "staged changes" and "comitted changes" don't really get submitted, you need to stage _then_ commit.
- **Pull** (the ↓ button up top): This is how you get remote changes into your local repository. (this might not be working 100% right now, we're still looking into how obisdian-git interacts with forks, but we can talk about how to use github desktop to do this later.)

So the basic workflow when you've made changes is to stage them, then press commit, then press "push". Pushing is the only thing which actually _uploads_ changes. That means that if you learn more advanced usages of git you can for example _revert_ committed changes if you need to. But let's not worry about that right now.

So for now let's:
- Stage all
- Commit
- Push
