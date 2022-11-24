# Hands on Git Hub

This repository is meant to provide a short introduction to GitHub in an informal way. It is tailored for the different activities that we run in the lab rather than as a course. 

The readme file will point to existing popular resources such as [Git Hub skills](https://github.com/skills).

<details id=2>
<summary><h2>Description</h2></summary>

(Extracted from [Simplilearn platform](https://www.simplilearn.com/tutorials/git-tutorial))

![What is Git](https://github.com/esgomezm/hands_on_github/raw/main/images/whats_git.png)
![What is GitHub](https://github.com/esgomezm/hands_on_github/raw/main/images/whats_github.png)
   
</details>

<details id=2.1>
<summary><h2>How are GitHub accounts organized</h2></summary>

  - **Personal GitHub account**: is unique and the owner of the account is the only one who can manage it. A personal account can have both private and public repositories. In the free version, each personal account can have a personal webpage built on top of GitHub pages. 
   
    A GitHub profile is many times the portfolio of a software developer or a researcher. GitHub can keep track or your coding activity, interaction and contributions to others (issues, discussions, commits, pull request), so you may consider take some care of it. To enrich the information given in your profile, you can always [add a README to the main page](https://docs.github.com/es/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme).

  - **GitHub organizations**: Shared accounts where the lab (Henriques' lab) and open-source projects (BioImage.IO, Fiji, ImageJ2) can collaborate across many projects at once, with sophisticated security and administrative features. Teams usually work within organisations as it serves as a container for shared work and gives the work a unique name and brand.

Usually an organisation looks like this:
![GitHub Organisation](https://github.com/esgomezm/hands_on_github/raw/main/images/henriques_lab_organisation.png)

We can always see in the user's profile if they are part of any public organization:
![GitHub user with organisations](https://github.com/esgomezm/hands_on_github/raw/main/images/curtis_profile.png)
</details>

<details id=3>
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


<details id=4>
<summary><h2>What do you need to start?</h2></summary>

 - **Create a GitHub (https://github.com/) account**. The email can be changed in the future. It might be interesting to sign up as a member from an academical institution.
 - **Install Git locally**. Follow the guidelines [here](https://github.com/git-guides/install-git).

</details>

<details id=5>
<summary><h1>Tips building up a documented software repository</h1></summary>

   <details id=5.1>
   <summary><h2>Create a repo</h2></summary>

   <img src="https://github.com/esgomezm/hands_on_github/raw/main/images/create_repo.png" align="right" width="400"/>

   - Name: avoid using underscores (`_`) in the name. Changing the name of a repository in the future is not recommendable as all the links depend on this naming so take some time to think about it.
   - Public/Private: this is personal and depends on each project. Any of the choices are reversible.
   - README.md: It is the first thing that anyone will see when entering in your repo. It can be the main entry to the documentation of your code or the source to link other resources (webpages, wiki). It is a good place to link the code with any existing reference and to indicate how to cite the work.
   - .gitignore: it tells git which files or folders should not be tracked.
   - License: If you are developing some code that is expected to be public in the future, you shoudl always care about its license. GitHub has already the templates for many different licenses. The most common ones for open source are MIT, BSL3-Clause, BSL2-Clause, but the are plenty of them.
   </details>
   
   
   <details id=5.2>
   <summary><h2>Structure your repository</h2></summary>

   There are different ways of structuring software repositories depending on its use, programming language, dissemination points (conda, pip, maven).

   Here are some examples of well documented and installable repositories ([StarDist](https://github.com/stardist/stardist), [NanoJ SRRF](https://github.com/HenriquesLab/NanoJ-SRRF), [scikit-image](https://github.com/scikit-image/scikit-image), [bioimageio core python](https://github.com/bioimage-io/core-bioimage-io-python), [bioimageio core java](https://github.com/bioimage-io/core-bioimage-io-java)).

   In general terms, the main folder of your repo should contain: 
   - Code folder. In Java, it is usually src. In Python it usually has the name of the package we are building, as it is the one we call in the code.
   - Folder with examples, tools, images or additional information.
   - Scripts to reproduce the environment (`environment.yaml`, `requirements.txt`, `setup.py`, `setup.cfg`).
   - README.md
   - LICENSE

   </details>
   
   <details id=5.3>
   <summary><h2>Update your repository</h2></summary>
   
   - [Commits](https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/about-commits): The most basic way to update a repository. They are small groups of meaningful changes. Basically, you change something in your files, register the changes and update the repository. While we can always check old code, commits are irreversible. This is why many times we work with pull requests.
   - [Pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests): It can gather a number of commits (registered changes in your code) or it is a way to contribute to someone's main code. They are used when the code needs to be changed considerably but the updates might be unstable, to work on aa general update or collaborate with someone's code. Indeed, this is the only way to contribute to someone's code when you do not have permissions to change it. A very nice feature of Pull Requests is that they allow discussions and reviews.
   - [Branches](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches): GitHub repositories are organised in branches. The repository always has at least the main branch and then you can create additional ones wihout affecting the main code. They are quite useful when an exiting code is under development and you are actively working with it, as it does not disturb the main repository. Usually, we work on the branch and once the code is ready to be updated, we open a pull request to merge its content with the main repository.
   - [Tags](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/managing-commits/managing-tags): Tags are associated with commits, so you can use a tag to mark an individual point in your repository's history, including a version number for a release.
   
   </details>
  
   <details id=5.4>
   <summary><h2>Packaging your repo and track of versions</h2></summary>
    
   Releases are created once a repo is ready to be used, distributed or to set a version:
   - [Releases](https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases): They package the repository and also allow including additional files for distribution. Releases are always associated with a branch and they always createa tag to mark a specific point in the repository's history. It is recommendable to build the version on top of the main branch. 
   
   </details>
</details>


<details id=x>
<summary><h1>Topics to explore and comment during the session</h1></summary>

- Issue tagging and assignments
- Workflows and continuous integration
- Organisation projects 
</details>
