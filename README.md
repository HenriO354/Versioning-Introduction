# Versioning-Introduction
  What is “version control” ?
  Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later.
  
##  Getting Started with Git and GitHub 
##  - Git vs GitHub ?
      Git is software for tracking changes in any set of files, usually used for coordinating work among programmers collaboratively developing           source code during software development.
      
      Whereas GitHub,is a provider of Internet hosting for software development and version control using Git. The main purpose of GitHub is to           facilitate the version control and issue tracking aspects of software development.

##   - Installing Git on Linux ( Debian/Ubuntu )

       For the latest stable version for your release of Debian/Ubuntu
       apt-get install git
       
##   - Installing on Windows

       The most official build is available for download on the Git website. Just go to https://git-scm.com/download/win and the download will            start automatically.
       
##   - Git Settings

       You can specify Git configuration settings with the git config command in a text editor (nano, atom, NeoAtom, VsCode) as it follows:
       $ git config --global user.name "John Doe"
       $ git config --global user.email johndoe@example.com
       
##   - GitHub Settings
        ## About SSH key generation
        
        You must generate a new SSH key to use for authentication as it follows:     
        
        Open Terminal
        Paste the text below, substituting in your GitHub email address
        $ ssh-keygen -t ed25519 -C "your_email@example.com"
        output:
        
        > Generating public/private algorithm key pair.
        > Enter a file in which to save the key (/home/you/.ssh/algorithm): [Press enter]
        > Enter passphrase (empty for no passphrase): [Type a passphrase]
        > Enter same passphrase again: [Type passphrase again]
        
        When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.
        
        ## Adding your SSH key to the ssh-agent
        
        Start the ssh-agent in the background:
        $ eval "$(ssh-agent -s)"
        > Agent pid 59566
        
        ## Add your SSH private key to the ssh-agent:
        
        $ ssh-add ~/.ssh/id_ed25519 ( replace id_ed25519 in the command with the name of your private key file )
        
        ## Copy the SSH public key to your clipboard.

        $ cat ~/.ssh/id_ed25519.pub
          Then select and copy the contents of the id_ed.pub file displayed in the terminal to your clipboard
        
        ## Go to GitHub.com and login
        
        Click the green “New Repository” button
        Repository name: myrepo
        Public
        Check Initialize this repository with a README
        Click the green “Create repository” button
        Copy the HTTPS clone URL to your clipboard via the green “Clone or Download” button.
       
        ## Clone the repository to your computer
        
        Determine where you are in the file directory (pwd). cd to move around. You can clone this repository wherever you want, though eventually         you’ll want to develop a system for storing your repos in a consistent manner.
        
        Clone myrepo from GitHub to your computer. Cloning simply downloads a copy of the repository to your computer.Remember the URL youcopied!
        ( GitHub username + the name of your practice repository )
        Type the git command: git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git                

##   - Cheat-Sheet    
    
    [git-cheat-sheet-education.pdf](https://github.com/HenriO354/Versioning-Introduction/files/8484153/git-cheat-sheet-education.pdf)
    
##   - Sources



