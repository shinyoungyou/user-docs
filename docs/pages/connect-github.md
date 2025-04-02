# Connecting to GitHub

## Overview
In this section, we will explore how to connect VS Code to GitHub seamlessly. This guide demonstrates how to connect GitHub to your VS Code workflow, allowing you to manage repositories, commit changes, and push code directly from the editor. By following these steps, you'll streamline version control and enhance collaboration, enabling you to focus on building projects.

## Option 1: In VS Code
In this option, we assume that you already know how to create a new, empty folder on your computer and you have installed Git.
<br>

### Open a folder and Create a file
1. Click the first icon (Explorer section) in the left navigation, and open a folder you want to save files.

    <figure markdown="span">
      ![Image title](images/step1.jpg){ width="100%" }
    </figure>

2. In the Explorer section, click the one paper icon (New File...) to create a new file.

    <figure markdown="span">
      ![Image title](images/step2.jpg){ width="100%" }
    </figure>
!!! success
    The folder has been opened and the new file has been created.

<h3 id="custom-anchor">Open a new terminal and Type commands</h3>

1. In the top navigation, click the terminal option and the new terminal.

    <figure markdown="span">
      ![Image title](images/step3.jpg){ width="100%" }
    </figure><br>

2. Type the command below to initialize a local Git repository in the terminal
> git init
!!! success
    The new terminal has been opened and some commands have been written.

### Create a GitHub repository in the VS Code
1. Click the third icon(Source Control) in the left navigation

    <figure markdown="span">
      ![Image title](images/step5.jpg){ width="100%" }
    </figure>
  
2. Click the Publish Branch button

    <figure markdown="span">
      ![Image title](images/step6.jpg){ width="100%" }
    </figure>
    !!! warning
        If you can't find "Publish Branch" button, please check the Troubleshooting section.

3. Click the Allow button, and sign in using GitHub

    <figure markdown="span">
      ![Image title](images/step7.jpg){ width="100%" }
    </figure>

4. Choose whether to make the repository public or private

<figure markdown="span">
  ![Image title](images/step8.jpg){ width="100%" }
</figure>
!!! success
    The new GitHub repository has been created.

<br>

## Option 2: From GitHub
In this option, we assume that you already have a GitHub account and have installed Git.
<br>

### Create a new repository in the GitHub
1. Open the GitHub and sign in

    <figure markdown="span">
      ![Image title](../assets/github1.gif){ width="100%" }
    </figure>

2. Choose "Your repositories" clicking your profile image and click "New" green button

    <figure markdown="span">
      ![Image title](../assets/github2.gif){ width="100%" }
    </figure>

3. Write a new repository name and check the "Add a README file" section

    <figure markdown="span">
      ![Image title](../assets/github3.jpg){ width="100%" }
    </figure>
    !!! note
        If you want to make the repository private, choose "private" option

4. Click "Create repository" green button in the bottom

    <figure markdown="span">
      ![Image title](../assets/github4.jpg){ width="100%" }
    </figure>
    !!! success
        The new GitHub repository has been created in the Github.

### Clone the GitHub repository to the VS Code
1. Click "<>Code" green button

    <figure markdown="span">
      ![Image title](../assets/github5.jpg){ width="100%" }
    </figure>

2. Click the icon highlighted in the red box below to copy the link

    <figure markdown="span">
      ![Image title](../assets/github6.jpg){ width="100%" }
    </figure>

3. In the VS Code, open a new terminal and type the command below to clone the GitHub repository
> git clone THE COPIED LINK FROM GITHUB

    !!! note
        If you don't know how to open a new terminal, click the below sentence.
        <br>
        [Open a new terminal and Type commands](#custom-anchor)

    !!! success
        The GitHub repository has been cloned to the VS Code.
