# Test Setup

Primary aim: document steps to test the "MarkPub Quickstart"
instructions.  


1. Make a directory and populate with some Markdown documents.


2. OPTIONAL: Make it an Obsidian vault  
DONE: create some wiki-links ...  
TODO: install ObsidianGit plugin  
 - note: ObsidianSync plugin enabled by default?  - DISABLE

3. Make it a GitHub repository  
TODO: put the CLI steps here  
 - note: a GitHub repository MUST be created before adding content.
 - one way to do this: manually create an empty repository on GitHub.com first. Do not initialize it with a README, license, or .gitignore files when creating it on GitHub, as you're pushing an existing repository.  
 - TODO: decide about specifying README, etc. on GitHub.com or in the document collection.
 - CLI steps:  
 ```shell
 # 1. Navigate to the document collection directory
cd your-document-collection

# 2. Initialize a new git repository
git init

# 3. Add all files to staging
git add .

# 4. Commit the files
git commit -m "Initial commit"

# 5. Create a new repository on GitHub (you'll need to do this manually on GitHub.com)
# Then, add the remote repository URL
git remote add origin https://github.com/username/repository-name.git

# 6. Rename the default branch to 'main' (if needed)
git branch -M main

# 7. Push your code to GitHub
git push -u origin main
```

4. MarkPub initialization  

5. Netlify setup?  

6. Test deployment  

TODO: separate this into two documents  
- one for pre-MarkPub install and init  
- one to test the MarkPub install and use instructions  

-----
2025-02-04: testing a simple GitHub pages deployment:  
 (1): directory previously set up as a GitHub repository  
 (2): `markpub init directory-name`  
```shell
cd directory-name
git add .
git commit -m "MarkPub initialization"
git push
```  
 (3): copied `.github/` directory from an existing document-collection
 repository  
   - edited the `.github/workflows/gh-pages.yml` file and inserted
     this repository's name into the `markpub build ...` command  
```shell
git add .github/
git commit -m "GitHub pages config files"
git push
```  
 (4) logged into GitHub, and for this repository's "Pages" settings,
 set "Build and deployment" "Branch" to "gh-pages" in the drop-down
 menu, and "Save" that setting  
  - Saving that setting triggers and "pages build and deployment"
    workflow under the "Actions" tab  
  - when completed the website is available at:  
  <https://githubaccountname.github.io/repositoryname>  
  (in this example this is https://band.github.io/mptestcollection)  


