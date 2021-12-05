# ✨ mySite ✨

Created with <a href="url">Velo</a>

You can clone your site code locally and work on any IDE.

## Quick Setup 🏎

In order to start code locally, run the following:

1. Clone your site:

       git clone <your-repository-url>
       
2. Open your site directory:

       cd <site-directory>
       
3. Set up your environment:

       npx velo init


## Develop Locally 📝

In the project directory, you can:

Fetch continuously online changes in real time to you local environment.

       npx velo get-ui-changes --watch
       
Open the editor preview mode running your local code changes and the current UI version from the online editor. 

       npx velo open-preview
       
Open a test site running your local code changes and the current UI version from the online editor. 

       npx velo open-test-site

<hr>

Once your code is ready use <code>commit</code> and <code>push</code> git commands to stream your local changes back to the editor to make them available to your team members.

## Editor Operation that modify code ⚠️

When the designer working online makes operations that modify code, the editor will commit and push the following changes to the master branch:
1. Add new page
2. Duplicate page with code
3. Delete page

## Learn More

You can learn more in our <a href="url">Help Center Documentation</a>
