# Hands on Git Hub

This repository is meant to provide a short introduction to GitHub in an informal way. It is tailored for the different activities that we run in the lab rather than as a course. 

The readme file will point to existing popular resources such as [Git Hub skills](https://github.com/skills) or [GitHub docs](https://docs.github.com/en).

<details id=0>
<summary><h2>Basic documentation</h1></summary>

<details id=1>
<summary><h2>Description</h2></summary>

(Extracted from [Simplilearn platform](https://www.simplilearn.com/tutorials/git-tutorial))

![What is Git](https://github.com/esgomezm/hands_on_github/raw/main/images/whats_git.png)
![What is GitHub](https://github.com/esgomezm/hands_on_github/raw/main/images/whats_github.png)
   
</details>

<details id=1.1>
<summary><h2>How are GitHub accounts organized</h2></summary>

  - **Personal GitHub account**: is unique and the owner of the account is the only one who can manage it. A personal account can have both private and public repositories. In the free version, each personal account can have a personal webpage built on top of GitHub pages. 
   
    A GitHub profile is many times the portfolio of a software developer or a researcher. GitHub can keep track or your coding activity, interaction and contributions to others (issues, discussions, commits, pull request), so you may consider take some care of it. To enrich the information given in your profile, you can always [add a README to the main page](https://docs.github.com/es/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme).

  - **GitHub organizations**: Shared accounts where the lab (Henriques' lab) and open-source projects (BioImage.IO, Fiji, ImageJ2) can collaborate across many projects at once, with sophisticated security and administrative features. Teams usually work within organisations as it serves as a container for shared work and gives the work a unique name and brand.

Usually an organisation looks like this:
![GitHub Organisation](https://github.com/esgomezm/hands_on_github/raw/main/images/henriques_lab_organisation.png)

We can always see in the user's profile if they are part of any public organization:
![GitHub user with organisations](https://github.com/esgomezm/hands_on_github/raw/main/images/curtis_profile.png)
</details>

<details id=2>
<summary><h2>When do we use GitHub?</h2></summary>

### Examples of GitHub usage in the lab or in science:
- Collaborative or individual software projects (NanoJ, ZeroCostDL4Mic, BioImage Model Zoo, deepImageJ...)
- Methods (scripts for data analysis, pipelines, software components of a book chapter)
- Webpages
- Paper writting (*e.g.*, connect with Overleaf)
- Course materials
- Slides if they are programmable (ImJoy slides)

### GitHub is NOT 
- A data storage
</details>

<details id=3>
<summary><h2>Why should you consider using GitHub?</h2></summary>

GitHub keeps record of the changes in your code and your activity. Therefore, it is a way to get back to previous code without storing different packages and to avoid messing up your developments. Moreover, it enables a more organised way of collaborations. It can keep track of the versions. For paper writting, it enables switching between templates and versions, and compare between different contributions. It is also a way to prove your contributions to a project and measure your activity. 

</details>

<details id=4>
<summary><h2>What do you need to start?</h2></summary>

 - **Create a GitHub (https://github.com/) account**. The email can be changed in the future. It might be interesting to sign up as a member from an academical institution.
 - **Install Git locally**. Follow the guidelines [here](https://github.com/git-guides/install-git).

</details>

<details id=5>
<summary><h2>Tips building up a documented software repository</h2></summary>

   <details id=5.1>
   <summary><h3>Create a repo</h3></summary>

   <img src="https://github.com/esgomezm/hands_on_github/raw/main/images/create_repo.png" align="right" width="400"/>

   - Name: avoid using underscores (`_`) in the name. Changing the name of a repository in the future is not recommendable as all the links depend on this naming so take some time to think about it.
   - Public/Private: this is personal and depends on each project. Any of the choices are reversible.
   - README.md: It is the first thing that anyone will see when entering in your repo. It can be the main entry to the documentation of your code or the source to link other resources (webpages, wiki). It is a good place to link the code with any existing reference and to indicate how to cite the work.
   - .gitignore: it tells git which files or folders should not be tracked.
   - License: If you are developing some code that is expected to be public in the future, you shoudl always care about its license. GitHub has already the templates for many different licenses. The most common ones for open source are MIT, BSL3-Clause, BSL2-Clause, but the are plenty of them.
   </details>
   
   
   <details id=5.2>
   <summary><h3>Structure your repository</h3></summary>

   There are different ways of structuring software repositories depending on its use, programming language, dissemination points (conda, pip, maven).

   Here are some examples of well documented and installable repositories ([StarDist](https://github.com/stardist/stardist), [NanoJ SRRF](https://github.com/HenriquesLab/NanoJ-SRRF), [scikit-image](https://github.com/scikit-image/scikit-image), [bioimageio core python](https://github.com/bioimage-io/core-bioimage-io-python), [bioimageio core java](https://github.com/bioimage-io/core-bioimage-io-java)).

   In general terms, the main folder of your repo should contain: 
   - Code folder. In Java, it is usually src. In Python it usually has the name of the package we are building, as it is the one we call in the code.
   - Folder with examples, tools, images or additional information.
   - Scripts to reproduce the environment (`environment.yaml`, `requirements.txt`, `setup.py`, `setup.cfg`).
   - README.md
   - LICENSE
   - Wiki (optional): it's a collection of markdown files meant to document the repository. It can be used as user guidelines or documentation for the collaborators of the repository. It's an alternative to the README.md for a more extended content. Check out [ZeroCostDL4Mic](https://github.com/HenriquesLab/ZeroCostDL4Mic/wiki).

   </details>
   
   <details id=5.3>
   <summary><h3>Update your repository</h3></summary>
   
   - [Commits](https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/about-commits): The most basic way to update a repository. They are small groups of meaningful changes. Basically, you change something in your files, register the changes and update the repository. While we can always check old code, commits are irreversible. This is why many times we work with pull requests.
   - [Pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests): It can gather a number of commits (registered changes in your code) or it is a way to contribute to someone's main code. They are used when the code needs to be changed considerably but the updates might be unstable, to work on aa general update or collaborate with someone's code. Indeed, this is the only way to contribute to someone's code when you do not have permissions to change it. A very nice feature of Pull Requests is that they allow discussions and reviews.
   - [Branches](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches): GitHub repositories are organised in branches. The repository always has at least the main branch and then you can create additional ones wihout affecting the main code. They are quite useful when an exiting code is under development and you are actively working with it, as it does not disturb the main repository. Usually, we work on the branch and once the code is ready to be updated, we open a pull request to merge its content with the main repository.
   - [Tags](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/managing-commits/managing-tags): Tags are associated with commits, so you can use a tag to mark an individual point in your repository's history, including a version number for a release.
   
   </details>
  
   <details id=5.4>
   <summary><h3>Packaging your repo and track of versions</h3></summary>
    
   Releases are created once a repo is ready to be used, distributed or to set a version:
   - [Releases](https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases): They package the repository and also allow including additional files for distribution. Releases are always associated with a branch and they always createa tag to mark a specific point in the repository's history. It is recommendable to build the version on top of the main branch. 
   
   </details>
</details>

<details id=6>
<summary><h2>Interaction with other repositories</h2></summary>

 - **Download**. All the respositories to which one has access (public or private) can be downloaded. 
 - **Fork**. Ideally, when one ones to build a new software upon an exisiting one or to contribute to it considerably. It will create a new repository in our github account but it will keep track of the repository previous history.

</details>

</details>

<details id=7>
<summary><h2>Practicals</h1></summary>

## Practical Exercise 1: first contact :hatching_chick:

(Based on the introductory course of [GitHub skills](https://github.com/skills/introduction-to-github))

1. Open a new browser tab, and work on the steps in your second tab while you read the instructions in this tab.
2. Create a repository with your account (for example, one related to the main project you are working on). It can be Private.
3. Click on add file:
      
      3.1. If you have something to upload --> upload files. Upload a file, a entire code (t will preserve the directory structure you have) or whatever you want. Choose `create a new branch` before accepting
      
      3.2. If you do not have anything, choose add file and name it as `README.nmd`. GitHub can only create markdown (.md) files. Write something like: `This is going to be your first repository :blush:`. Choose `create a new branch` before accepting

5. It will suggest to open a pull request. Do not do it! We are going to explore a bit more. Go to the main page of the repo and choose the new branch. 
6. Change something in one of the files (either uploading or clicking on edit in the README file). Push the commit.
7. Open the **pull requests** tab.
8. Click on **compare & pull request**. It will suggest which branches to compare (the new one with the main, in this case).
9. In this pull request, go to the **Files changed** tab. Here you can review the changes or edit the files. 
10. Select **Edit file** from the three dotted **...** menu in the upper right corner of one of the files (e.g., `README.md`) and add some information. For example, a new line with `You are becoming an expert :hatched_chick:`.  
12. Above your new content, click **Preview**.
13. At the bottom of the page, type a short, meaningful commit message that describes the change you made to the file.
14. Click **Commit changes**.
15. Wait about 20 seconds then refresh this page for the next step.
16. Get back to the **Conversation** tab and click on **merge pull request**. Write something if you consider it is important. 
17. Click on **close**.
18. In the **Settings** tab of your repository, you can see all the activity. 

## Practical Exercise 2: keeping track of your writting :rooster:

1. Got to the [LateX template in Henrique's lab](https://github.com/HenriquesLab/HenriquesLab-bioRxiv-template/tree/main).
2. Fork the repository in your account.
3. Go to Overleaf and open a new project with `Import from GitHub`. It may ask you about your GitHub user information. Chose the repository that you just forked.
   <img src="https://github.com/esgomezm/hands_on_github/raw/main/images/import_from_github.png" align="center" width="200"/>
   <img src="https://github.com/esgomezm/hands_on_github/raw/main/images/choose_repo_overleaf.png" align="center" width="400"/>
   
4. Change something in the document (the title for example). 
5. In the menu of the document, click on GitHub. It will ask you whether you want to push the changes (i.e., update the repository in your account).
6. Add a title to your commit and push it. 

   <img src="https://github.com/esgomezm/hands_on_github/raw/main/images/connect_with_github_overleaf.png" align="center" width="200"/>
   <img src="https://github.com/esgomezm/hands_on_github/raw/main/images/push_changes_overleaf.png" align="center" width="300"/>
   <img src="https://github.com/esgomezm/hands_on_github/raw/main/images/commit_title_overleaf.png" align="center" width="300"/>
7. In GitHub, create a release. The tag name will be the one used as a reference for searching commits in the code. Ideally you will have different commits. You can register your supervisor's comments, rebuttals, changes in the bibliography so you can work together with your colleagues and even update your Mendeley or Zotero libraries. 

   <img src="https://github.com/esgomezm/hands_on_github/raw/main/images/release.png" align="center" width="450"/>
   <img src="https://github.com/esgomezm/hands_on_github/raw/main/images/draft-release.png" align="center" width="450"/>

8. Get back to previous versions of your paper.

   <img src="https://github.com/esgomezm/hands_on_github/raw/main/images/choose-tag.png" align="center" width="300"/>
   <img src="https://github.com/esgomezm/hands_on_github/raw/main/images/recover_code.png" align="center" width="500"/>


</details>

## Topics to explore and comment during the session

- Issue tagging and assignments
- Workflows and continuous integration
- Organisation projects 

