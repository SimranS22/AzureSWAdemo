<div align="center">
<h1>Azure Static Web Apps</h1>
</div>
<div align="center">
<img width="878" alt="Event Poster" src="https://user-images.githubusercontent.com/103310345/218158083-6724960b-bab1-4b75-8b4a-8e0040e76f79.png">
</div>


As a _Microsoft Learn Student Ambassador_, I had the opportunity to conduct a Hands-on Session/workshop on 7th Jan,2023 on "**Introduction to Azure Static Web Apps**".

### Aim

To help people understand how to deploy static web apps using Azure.

### Workshop Details

This workshop covers the following topics :
1. Introduction to Static Web Apps
2. Features of Static Web Apps
3. Deploy a Static Web App - Hands-on session

**Check out the workshop here :**

<a href="https://stdntpartners-my.sharepoint.com/:v:/g/personal/desmond_dadzie_studentambassadors_com/EQfJMHbxwQxJl58K7z-LOyoBAkSd_wUbEoGngbI3W_qRiw?e=DnTakd">Introduction to Azure Static Web Apps</a>


# Documentation

A step-by-step documentation of how to deploy your very own static web app using Azure.


## Prerequisites 

To get started, complete the following items if you haven’t already 

- Create a [GitHub](https://github.com/) account  

- Create an Azure for Students account or use your existing Azure Subscription if you have one.

- Download [Visual Studio Code](https://code.visualstudio.com/Download) and the [Azure Static Web Apps extension](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-azurestaticwebapps) for Visual Studio Code 

- Download [GitHub Desktop](https://desktop.github.com/)  

## Step 1: Create a repository 

This article uses a GitHub template repository to make it easy for you to get started. The template features a starter app used to deploy using Azure Static Web Apps. 

1. Navigate to the following location to create a new repository: [https://github.com/SimranS22/AzureSWAdemo/generate](https://github.com/SimranS22/AzureSWAdemo/generate) 

2. Name your repository *AzureSWAdemo*. Note: Azure Static Web Apps requires at least one HTML file to create a web app. The repository you create in this step includes a single index.html file. 

3. Select Create repository from template. 

## Step 2: Clone the repository 

Previously you created a GitHub repository that housed the materials needed to create your web app.  Now you’ll create a local copy (or clone) so you can modify the code on your system. Cloning repos is an important part of a developer’s work. Imagine you’re a software engineer in a large company, and all the engineers at your company are working on the same codebase. You wouldn’t want everyone to make changes to the source code at the same time – so everyone clones the source code to their own local repository, makes and tests the necessary changes, and pushes those changes to the source code when they are ready. This makes for greater organizational collaboration. 

1. Open the GitHub Desktop App 

2. Navigate to File > Clone Repository 

3. Open the URL tab 

4. Input https://github.com/<YOUR_GITHUB_ACCOUNT_NAME>/AzureSWAdemo.git into the URL input, and select Clone 

Note: Make note of the location where the repository is saved.  

## Step 3: Create a Static Web App 

With the copy created locally, you’re all set to start working on your code and site. Now you’ll explore how to deploy your site to the cloud. You’ll use Azure Static Web Apps to host your site. A static web app (SWA) is a site built with JavaScript, HTML, CSS and potentially other tools, and SWAs are becoming increasingly common. Using Azure Static Web Apps will allow you to quickly post your site to the world. You can explore more Azure Tips and Tricks: Static Web Apps to learn more.  

1. Open Visual Studio Code and go to File > Open Folder to open the cloned repository in the editor.  

2. Inside Visual Studio Code, select the Azure logo in the Activity Bar to open the Azure extensions window. 

- Note: You are required to sign in to Azure and GitHub in Visual Studio Code to continue. If you are not already authenticated, the extension will prompt you to sign in to both services during the creation process. 

3. Under the Static Web Apps label, select the plus sign. 

4. The command palette opens at the top of the editor and prompts you to select a subscription name. Select your subscription and press <Enter>. 

5. Next, name your application. Type AzureSWAdemo and press <Enter>. 

5. Select a region close to you. 
- Note: Azure Static Web Apps globally distributes your static assets. The region you select determines where your optional staging environments and API function app will be located. 

6. Select Custom  Enter /src as the location for the application files and press <Enter>. This app does not produce a build output. Ensure the build output location is empty and press <Enter>. 

7. Select “Open Actions in GitHub.” This will launch the GitHub Actions tab in your browser. You will see the workflow run as it is creating the app. When your webapp is built and deployed, you will see a check for the workflow run.   

- Once the app is created, navigate back to Visual Studio Code - a confirmation notification is shown there. The Visual Studio Code extension also reports the build status to you as the deployment is in progress – and will update you when your app is built and deployed.  

- Once the deployment is complete, you can navigate directly to your website. 

8. To view the website in the browser, right-click on the project in the Static Web Apps extension, and select Browse Site. 

If your build has failed you may see this in your Actions tab on GitHub:
 
 ![Failed build in GitHub actions](https://user-images.githubusercontent.com/32169182/175279158-50787c0d-2c28-4140-9724-0449023e8ae1.png)
 
 To fix this you can click the pencil icon beside the workflow run and click View workflow file
 
 ![View workflow file](https://user-images.githubusercontent.com/32169182/175279494-92985faa-a4aa-42b1-8f61-50cf5032816a.png)
 
 Then change line 30 to be /src instead of /
 
 ![Change app location](https://user-images.githubusercontent.com/32169182/175279576-fc87decb-99d0-41b7-8be3-ab9a56d9ca2a.png)

## Step 4: Customize Your Static Web App 

With your app deployed, you can turn your attention to customizing the app.

We will now do a small customization step customize your webapp you can edit it in VS Code and push changes using GitHub Desktop  

1. Navigate to the Explorer Tab in Visual Studio Code   

2. Navigate to the “src” folder, and within it, any file such as "index.html"

3. Make a change such as changing the word "lorem" to "HELLO" in the paragraph   

4. Save your changes in VS Code   

5. Navigate to GitHub Desktop and ensure that your Current Repository is your AzureSWAdemo repo (GitHub Desktop should reflect your recent changes like below)  

6. In the bottom left of GitHub Desktop, give your changes a title (like “Changed text in paragraph” and add a description  

7. Select “Commit to Main”  

8. Now, push your changes to GitHub by selecting “Push Origin”    
  
9. Navigate to Actions in GitHub and view your web app’s build progress  

10. When the build is complete, refresh your app and the changes should be reflected  

