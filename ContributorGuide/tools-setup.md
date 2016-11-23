# Tools setup

## Install Git

There are several ways to install Git on your local computer.  Chose a method that works best for you. If you are unfamiliar with Git, the following is one way to install it.

1. Install [Software Freedom Conservancy's Git](https://git-scm.com/download) on your computer. This installs the Git version control system. It includes command-line integration options you use to interact with your local Git repository. Clients are available for Windows, MacOS, Linux, and Solaris. 

2. During install, you can accept all default settings unless you want different behavior.

> Note: If you prefer a Graphical User Interface over a Command Line Interface, see [Software Freedom Conservancy's available GUI Clients page](https://git-scm.com/downloads/guis), [GitHub's GitHub Desktop](https://desktop.github.com/), or [Visual Studio Code](https://www.visualstudio.com/products/code-vs.aspx) for some popular options. In this guide, we focus on using the command line interface.

## Configure your user name and email

To ensure you are listed correctly as a contributor, you need to configure your user name and email locally in Git.

1. Launch the Git enabled command prompt. For example, on Windows use *Git bash*, on MacOS use *terminal*, on Linux use *bash* shell.

2. Configure your user name so it matches your name as you set it up in your GitHub profile:

    ````
    git config --global user.name "John Doe"
    ````
3. Configure your email so it matches the primary email designated in your GitHub profile.

    ````
    git config --global user.email "alias@mycompany.com"
    ````
4. Type `git config -l` and review your local settings to ensure the user name and email in the configuration are correct.

## Install a markdown editor
Content is authored in a simple *markdown* notation rather than *markup* (HTML, XML, etc.). You can use any text based editor to edit and contribute in markdown. There are several editors that provide functionality for authoring markdown. The following is a list of popular markdown editors.

- **[Atom](https://atom.io)** - GitHub's Atom markdown editor. 
- **[Visual Studio Code](https://www.visualstudio.com/products/code-vs.aspx)** - Microsoft's lightweight cross platform editor. 

> Note: In some cases, bash launches an editor. For example, if you forget to add a commit comment.  By default, the editor is vi. If you want a different default editor, see [Associating text editors with Git](https://help.github.com/articles/associating-text-editors-with-git/) for details.

## Next steps

- [Git and GitHub repository initial setup](git-and-github-repository-initial-setup.md)
- Back to [contributors guide](./index.md)
