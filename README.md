
# How to host a Resume with jekyll theme on Github Pages using MacOs.

## Purpose

Get job offers from employers by impressing them with my Resume.

## Prerequisite

-   [Github acount](https://docs.github.com/en/get-started/signing-up-for-github/signing-up-for-a-new-github-account)
    
-   [Gem](https://sourabhbajaj.com/mac-setup/Ruby/RubyGems.html) installed
    
-   [Homebrew](https://brew.sh/) installed
    
-   [VSCode](https://formulae.brew.sh/cask/visual-studio-code) installed
    
-   Resume written in markdown
    

  

## **Part 1**: Creating resume using a template that uses jekyll theme.

  

 **1. Install Ruby using Ruby Version Manager (RVM)**
			
	 a)Open Terminal using Cmd+space.
	    
	 b)Type terminal and press enter which will open a new terminal.
	    
	 c)Type `\curl -sSL https://get.rvm.io | bash -s stable --ruby` in the terminal  and press enter.
    
 **2. Install Jekyll**
  

	 a)Type `gem install jekyll in the terminal and press enter.

    
   **3. Download a Theme**
 -  Select a theme you’d like to use for your resume by going to [Rubygems'](https://rubygems.org) site, which is a perfect place to find hundreds of themes to use for your markdown file along with some ready to use Projects, which can be modified as per your need.
    
 -  Search for `Resume Jekyll` via the search box.
    

	> Note: You can modify the words inside the quotes to search for
	> different themes, but make sure the theme is compatible with Jekyll.
	> One way to find if the theme is supported is to look for the word
	> “Jekyll” in the subtext below the name of the theme.

 -  Select any Jekyll theme you like from the result.
    
 -  Click on the `HomePage` link on the right-side of the webpage, which will redirect you to the theme’s Github Page which contains information on how to use the theme in your project.
    
 -  Scroll down until you see the `“README”` section. This section will contail relevant information on how to download the project on your Computer and how to modify the files so that the resume can be configured to display your details.
    
 -  Open the project using Visual studio code (VSCode).
    

> If you do not have VSCode installed please follow the steps below

		**Installing VSCode**
		
		1.  Download Visual Studio Code for macOS from the VSCode website.
		    
		2.  Unzip and launch the app.
		    
		3.  Drag the Visual Studio Code icon to the Applications folder.
		    
		4.  Add VS Code to your Dock by right-clicking on the icon and choosing Options, Keep in Dock.
		    
		5.  Launch VS Code by double-clicking on the icon in the Applications folder or searching for it with Spotlight.
		    
		6.  Click Open and select the project that you downloaded earlier from github.
		   
		7.  Click the View menu and select Terminal which will open a terminal at the bottom of VSCode.
		    
		8.  Type bundle install in the terminal window of VSCode and hit enter.
		    
		9.  Type bundle exec jekyll serve which should start a local server.
		    
		10.  Go to http://127.0.0.1:4000 in your browser and you should be able to see a resume in your webbrowser.
    
	Tip: The webpage automatically updates whenever the files of the project changes so you dont need to restart server everytime you make change to a file.**

-  Read the instruction in README section of the project’s github repository to edit the files with details of the resume markdown file you had created.
    
-  Save the files and check if the changes in the webpage reflect what you expected.
    

**Now you have a digital Resume that is ready to be uploaded in github pages.**

  

## Part 2: Uploading your Resume to github pages.

  

1) 	Setup Github Pages website.
	
		a.  Log in to your GitHub account and navigate to the main page.

		b.  In the top-right corner of the page, click the "+" icon, and then select "New Repository".

		c.  Give your repository a name, and then click "Create Repository".

		d.  On the next page, click "Settings".

		e.  In the "GitHub Pages" section, select "Master Branch" from the "Source" drop-down menu.

		f.  Click "Save".

    

2.  Edit your project settings so that it can be uploaded in github pages
    
		a.  Open the _config.yml file and set url to [your_github_username].github.io
		    
		b.  Set the baseurl to /[name_of_the_repository] you created.
    

> Note: Do not forget the “/” in the baseurl.

 3.  Upload the project to your github repository
    
			a.  Open a terminal in VSCode.
			    
			b.  Type `git init` and hit enter
			    
			c.  Type `git remote add origin https://github.com/[your_github_username]/[your_repository_name].git` and hit enter
			    
			d.  Type `git add .` and hit enter.
			    
			e.  Type `git commit -m “[any_message_you’d_like]”` and press enter.
			    
			e.  Type `git push -u origin main` and press enter.
	    

> Your GitHub Pages site will now be live at   
> http://[username].github.io/repositoryname, where "username" is your
> GitHub username, and "repositoryname" is the name of your repository.

  

## More Resources

-   [https://www.markdowntutorial.com](https://www.markdowntutorial.com) - Tutorial on how to create a markdown document.
    
-   https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS

-   at least one other resource
    

## Authors and Acknowledgements

-   [RyanxLoi](https://github.com/RyanxLoi)
    
-   P1
    
-   P2
    
-   p3
    

  
  

**FAQs**

 - As we know Markdown is eventually converted to HTML so why not use
   HTML directly?

	-   The main aim of using markdown is to abstract away the complexity of formatting text in web documents so that author can focus on the content instead. HTML can perfectly format the contents of the webpage but it has a steep learning curve. Markdown is very easy to learn and hence anyone with just little effort can write content for the web.
    

 - How do I know if a theme is compatible with Jekyll?

    

	-   A simple trick is to read the subtext under the theme’s name on the webpage and look for any word that says “Jekyll”.
    

-   I am getting an error when installing Ruby. What should I do?
    

	-   There are different other ways to install Ruby on your mac and one way is by using homebrew. You can refer the instruction in this [page](https://jekyllrb.com/docs/installation/macos/) for further instruction.
    

-   Clicking on homepage of the theme does not take me to github.
    
	
	-   In such case, instructions on how to install and configure the project can usually be found in the homepage of the template itself.
