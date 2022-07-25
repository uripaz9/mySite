# Wix CLI

Develop your site as a team using any IDE and Live Editor.

## Before Getting Started
Before getting started, make sure you have node 17 or above installed, as well as npm and Git.

## Setup 
To set up your local environment and start coding locally, run the following CLI commands in your terminal:

Clone your site 

  ```js
git clone <your-repository-url>
  ```

Navigate to your project directory

```js
cd <site-directory>
```

Run the ‘npm install’ command to add the necessary dependencies, including node packages, Velo CLI and the types folder necessary to support Velo auto-complete and error indications. Note that running this command may prompt you to log in to Wix. 

```js
npm install -g velo-cli-prototype
```

Start the Live Editor

```js
velo dev
```

Now you can start developing in your IDE. 

## UI version
UI version is the state of your site’s design, schemas and applications. Your code contains a reference to a UI version in the velo.config.json file. 
In order to sync your local code with the latest editor changes, done by you or others, click on ‘sync changes’ button in the Live editor. When you sync your local code with the latest UI version, you can address them in your code.

## Live Editor 
To make editor changes at the same time as editing local code, open the Live Editor by running 

  ```js
velo dev
  ``` 
The Live Editor will always run the latest Editor X UI version, which might be different from the UI version stated in your local code.To avoid errors, you should sync your changes in IDE to update to the latest UI version, by clicking on the ‘sync changes’ button in th Live Editor, or pressing ‘s’ in the velo CLI, before editing code.

 **Concurrent mode:**
 
When working with teammates, you will be working in concurrent mode. This means each change you make in the Live Editor will reflect to all other teammates, and vice versa. However, code changes in your IDE will not be updated to others until you push them to <code>origin/main</code>

 **Sync Live Editor changes into your IDE:**
 
You can sync your IDE changes with the ‘Sync Changes’ button in the editor top bar. This will ensure your local code is synchronized with the latest changes in the Editor X UI version.  

 **Sync code changes into the Live Editor:**
 
Hot reload - While ‘velo dev’ command is running, each time you edit code in your IDE, the Live Editor automatically updates with these changes.

## Online Editor
The Online Editor is tied to the <code>origin/main</code> branch, and updates automatically with the latest code change pushed to <code>origin/main</code>. Note that if an older UI version was pushed to git, this will not affect the UI version in the Online Editor.
Once the site is connected to GitHub, you’ll only be able to edit code in the external IDE. Code in the Online Editor will be in read-only mode.
The Online Editor will always reflect the most up to date UI version. 


## Preview Your local code changes 
When developing locally, you have 2 options to preview and test your local changes:

**1. Preview mode in Live Editor:**

By entering the preview mode in Live Editor you can see a preview of your site with your most current code and the latest Editor X UI version, interact with your site and debug your site’s code.

**2. Deploy preview:**

Create a new shareable version of your application or site in a production environment. This version will be based on your local code and the Editor X UI version stated in velo.config.json file.

  ```js
velo deploy-preview
  ``` 

## Go to Production 
To publish your local code changes, do the following: 

1 - <code>commit</code> and <code>push</code> your local code changes to <code>origin/main</code>. 
Note that the Editor is tied to the main branch, and updates with the latest code change pushed to <code>origin/main</code>.

2 - In order to publish your changes you have 2 alternatives:

Option A - Publish using the CLI:

Run ‘velo publish’ CLI command to publish the latest commit in origin master, and the editor UI version stated as part of this commit.

  ```js
velo publish
  ``` 

Option B - Publish using the the Publish button via the Online Editor:

Click Publish in the Online Editor. Note that clicking Publish in the Online Editor publishes the latest Editor X UI version, along with the latest code changes in the <code>origin/main</code> branch. 



## Invite Collaborators 
To allow other teammates access your github repository, edit code and make changes in the editor, you need to
Add them as Contributors to your site. Contributors need to be assigned the Admin role to be able to edit the site and the code. 
Invite them as collaborators on your github repository via Github. Note that you can have a different email address for Wix and Github accounts. Learn more https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository

### Learn More
See our [Help Center Documentation]() to learn more.





