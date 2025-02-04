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


