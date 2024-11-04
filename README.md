# How to make PDF documents with Pandoc

<!--toc:start-->
- [How to make PDF documents with Pandoc](#how-to-make-pdf-documents-with-pandoc)
  - [A quick reference to the Markdown syntax](#a-quick-reference-to-the-markdown-syntax)
  - [A brief introduction to LaTeX](#a-brief-introduction-to-latex)
  - [How to write Mermaid](#how-to-write-mermaid)
  - [Compiling your document with Pandoc](#compiling-your-document-with-pandoc)
  - [Neovim](#neovim)
  - [Version Control and Backup with Git](#version-control-and-backup-with-git)
    - [Installation](#installation)
    - [Usage](#usage)
  - [A brief tutorial for using GitHub and GitLab](#a-brief-tutorial-for-using-github-and-gitlab)
<!--toc:end-->



## A quick reference to the Markdown syntax
## A brief introduction to LaTeX
## How to write Mermaid
## Compiling your document with Pandoc
## Neovim
## Version Control and Backup with Git
### Installation
To use Git, first head to the [git's official website](https://git-scm.com/downloads) and download the latest version for 
your operating system. If you use a package manager, like APT, run the next command on your terminal to install it:
```shell
sudo apt install git
```

If you use NixOS, on your `/etc/nix/configuration.nix` add the following lines:
```nix
# /etc/nix/configuration.nix
environment.systemPackages = with pkgs; [
    git
];
```

### Usage
Open a terminal. Create a folder that will contain your files and move to it.
```shell
mkdir my-pdf
cd my-pdf
```

Then run the following command:
```shell
git init
```

This will start a new Git repository in that folder.
Git will watch for changes into that folder and save them whe you tell to do that.
Then let's create a simple `README.md` file with a "hello world":
```markdown
# Hello World!
```

To tell Git to add this to a "staging" list, run the following command:
```shell
git add README.md
```

Then, to tell git to register those changes run:
```shell
git commit -m "Create README.md"
```

Repeat the process with for every file that you have modified, and get the changes
registered and backed up locally by Git. You should be clear and concise with your
commit mesages (the one after th `-m` tag in the command).

## A brief tutorial for using GitHub and GitLab
