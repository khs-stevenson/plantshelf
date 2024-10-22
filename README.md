# 🌿PlantShelf  
In these 2 lessons, you will:  
* modify the structure (HTML) and style (CSS) of a webpage which shows image/information cards for different plants.  
* learn to use git and GitHub to back up and version-control your code.  

____
## **⯈Part A** git, GitHub, and HTML
### GitHub │ Forking a repository
GitHub is a website which stores files and all their past versions. The code for the PlantShelf webpage is currently stored in a folder (or *repository*) on GitHub, and your first step is to make your own copy of this folder on GitHub.

- [ ] Go to [GitHub.com](https://github.com/signup) and create a free account (or login if you already have one).  
- [ ] Go to [the PlantShelf repository](https://github.com/S-Mangan/plantshelf) and click Fork to create your own copy.

### Visual Studio Code │ Pulling from GitHub  
The next step is to get a local (i.e. on Windows) copy of your remote (i.e. on Github) repository. The tool we use for doing this is called `git`.  

- [ ] Open VisualCode, and open your home folder (File > Open Folder).
#### Set up git
* Open the terminal view (Terminal > New Terminal) and open a (gitbash? **TODO** check what's available) terminal.  

* Run these commands in your terminal to attach your name to your changes:  
> - [ ] `git config --global user.name "Your Name"`  
> - [ ] `git config --global user.email "your@email.com"`

* Run these commands in your terminal to create a secret key for your changes:  
    `$ ssh-keygen -t ed25519 -C "your_email@example.com"`   
    `$ eval "$(ssh-agent -s)"`   
    `$ ssh-add`  

* Tell GitHub about your secret key: 
**TODO screenshots**

#### Make your local copy
- [ ] Create local version of your PlantShelf copy: (**TODO** command details). 
    `git clone git@github.com:<your_github_username>/plantshelf.git `   
- [ ] Open the new local version (File > Open Folder > select plantshelf).

### Visual Studio Code │ Pushing to GitHub  
- [ ] Find the README.md file in the tree folder (View > Open View... > Folders), and put an `x` into the checkboxes (`[ ]`) you've completed.

#### Push the change
Back in your git bash terminal:  
- [ ] `git add README.md`  
- [ ] `git commit -m "Updated the readme"`  
- [ ] `git branch -M main  `  
- [ ] `git remote add origin git@github.com:<your_github_username>/plantshelf.git`  
- [ ] `git push`  

#### Check your change
- [ ] Refresh your plantshelf fork on GitHub. You should see your checked items in the README.

### Visual Studio Code │ Changing the HTML  
- [ ] Find the index.html file in the tree folder, and  
> - [ ] click and drag the index.html a browser window to see PlantShelf website  
> - [ ] double click index.html to see the HTML  

- [ ] Modify the HTML and refresh your browser to see how the website changes:  
> - [ ] Update the GitHub link in the footer to point to your fork.  
> - [ ] Replace some of the card images (see the images folder), and update the card headings to match.  
> - [ ] Change the main website heading  

## **⯈Part B** CSS
- [ ] **TODO** live server extension  
- [ ] **TODO** variables... try changing  
- [ ] **TODO** rem  
- [ ] **TODO** flex... flex-direction: column vs row    
- [ ] **TODO** grid... try changing gap,  grid-template-columns  
- [ ] **TODO** psuedo classes and transitions  
- [ ] **TODO** 


## [optional] Card flipping extension
* In the index.html, uncomment all the `<div class="back side">` sections, and in the head link the additional `flip_extension.css` stylesheet.  
* What happens now when you hover over a card?  
* Investigate the TODOs in `flip_extension.css` and try to make the cards flip.


## [optional] Further information and useful tools
#### YouTube │ Git in 15 Minutes
Watch [this YouTube video](https://github.com/signup) for a more detailed overview of git. Note that we didn't need to install git, and we don't need commands like `init`, `branch`, `checkout`, and `merge` for these lessons.  


#### Visual Studio Code │ Live Server extension
Search and install the Live Server extension (View > Open View... Extensions) and find out how to use it to automatically reload your webpage when you make a change
