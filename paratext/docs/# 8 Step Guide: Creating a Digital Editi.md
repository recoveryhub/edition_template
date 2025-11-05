# 8 Step Guide: Creating a Digital Edition

### <u>**Table of Contents**</u>
Step 1: Create a GitHub account <br>
Step 2: Create Template Edition <br>
Step 3: GitHub Repository: Setting Recommendations <br>
Step 4: Naming Your Project <br>
Step 5: Folder Structure & Organization <br>
Step 6: Configuring Your Edition Site <br>
Step 7: Publishing Your Edition <br>
Step 8: Updating Edition’s URL and Base URL <br>

#### <u>**Additional Considerations**</u>
Markdown Transcribing & Editing <br>
Troubleshooting

### <u>**Step 1: Create a GitHub account**</u>
[GitHub](https://github.com/) is a free, open-access resource that stores files that can run a website; it can also host that website thanks to a feature called [GitHub pages](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages). 

<u>If you do **not** have a GitHub account</u>, follow the [instructions on GitHub](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github) to create one.	

### <u>**Step 2: Create Template Edition**</u>

To get started with your own edition, you’ll need to create a GitHub repository for your project using our Recovery Hub edition template. 

First, visit the Recovery Hub’s [repository home page](https://github.com/recoveryhub/edition_template) [Fig. 1].

![Figure 1: Recovery Hub’s repository home page](https://)

Click the “Use this template” [Fig. 2] button at the top-right of the repository homepage, then select “Create a new repository” [Fig. 3] to copy it to your GitHub account.

![ Figure 2: “Use this template”](https://)   
![Figure 3: “Create a new repository”](https://)

After clicking on “Create a new repository,” GitHub will immediately take you to a page to set initial key settings for your new repository. Below, in <span style="color: #265095;">Step 3</span>, we share our setting suggestions.  


### <u>**Step 3: GitHub Repository Setting Recommendations**</u>

On the “Create a new repository” page [Fig. 4], you will be asked to choose your preferred repository settings. Below, we list the setting fields GitHub offers when creating a new repository along with our recommendations for each:

![Figure 4: GitHub New Repository Settings/Initial Setup Page](https://)

**Start with a template**: recoveryhub/edition_template

![start with a template](https://)

**Include all branches**: Off

![branches off](https://)

**Owner**: Keep your personal account selected unless your edition belongs to a specific GitHub organization.

![owner](https://)

**Repository Name**: Pick a name that is short but memorable (e.g., edition_test_km)

![repository name](https://)

Repository names <u>**cannot**</u> contain spaces, so we recommend using underscores in place of the spaces (e.g., edition_test_km). See <span style="color: #265095;">Step 4</span> for more on naming your project.

    
**Description**: Optional. You can always add or change later. 

![description](https://)

**Visibility**: It’s up to you. Either way, people will not be able to make changes without your approval.

> <u>**Private**</u>: Many people prefer to keep their repository private until the release is ready. If the repository is private, only the members you add will be able to see that it exists. To learn more about adding members, see <span style="color: #265095;">[inviting collaborators to a personal repository](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/repository-access-and-collaboration/inviting-collaborators-to-a-personal-repository)</span> in GitHub’s documentation.

>><u>**Public**</u>: To publish your edition with GitHub Pages, your visibility settings <u>**must**</u> be set to Public, which can be changed at any time. Refer to <span style="color: #265095;">Step 7</span> for instructions on updating visibility settings at a later time. 

![privacy](https://)

Once you’ve entered your initial settings, click “create repository” at the bottom of the page. 

It will take a few moments to set up your new repository. After it’s created, GitHub will automatically redirect you to your repository’s home page [Fig. 5]. 

>> <u>Note</u>: Your repository home page is what GitHub calls your repository’s “main branch.” The main branch is the primary and definitive version of the project's code, where you organize and store all your folders and files. In Figure 5, you’ll see it’s set as your repository’s default.

![Figure 5: edition_test_km Repository Home Page](https://)

### <u>**Step 4: Naming Your Project**</u>

Your project will use three types of naming conventions: a long name, a short name, and an edition prefix.

> **long name**: The project’s full edition title (e.g., Mary Johnston's The Wanderers: A Digital Edition).

> **short name**: The name for your edition’s GitHub repository. 

>> <u>**Note**</u>: The repository name can only contain upper and lowercase letters and underscores ( _ ). We recommend choosing two or three key words from your edition’s long name and using underscores where there would generally be spaces (e.g., johnston_wanderers).

> **edition prefix**: A brief unique identifier that precedes file names for your edition, which should be included every time you create and name a file.

Keep the prefix name basic and limited to five characters (numbers or letters) or fewer; it can indicate the edition’s version (e.g., ed1) or reflect the project's name.

ADD ADDITIONAL INFO

### <u>**Step 5: Folder Structure & Organization**</u>

There are several <span style="color: #63AEB6;">**main folders**</span> and <span style="color: #F7894E;">**subfolders**</span> you will primarily use. These folders will store various <span style="color: #E44C31;">**files**</span>, including but not limited to your documents, Markdown transcriptions, images, and more. 

In list form, using our color-coded **folder paths**, we explain what each folder contains, providing additional information as needed. 

<span style="color: #63AEB6;">**paratext**</span>: docs and essays subfolders

<span style="color: #63AEB6;">**paratext**</span>/<span style="color: #F7894E;">**docs**</span>: documentation materials

<span style="color: #63AEB6;">**paratext**</span>/<span style="color: #F7894E;">**essays**</span>: essays and other paratext that accompany your edition

<span style="color: #63AEB6;">**items**</span>: ready-to-publish Markdown transcriptions. You will upload Markdown-encoded documents (.md files) here manually.

> <u>Note</u>: If you are working with multiple genres, use the subfolders in <span style="color: #63AEB6;">**items**</span> to organize your files by genre. The sample files in the template are organized by <span style="color: #E44C31;">**books**</span>, <span style="color: #E44C31;">**periodicals**</span>, and <span style="color: #E44C31;">**poems**</span>.

<span style="color: #63AEB6;">**source**</span>: Markdown drafts, TEI drafts, Markdown sample files for built-in genres, and Ruby script

<span style="color: #63AEB6;">**source**</span>/<span style="color: #F7894E;">**drafts**</span>: Markdown drafts and TEI drafts 

> <u>Note</u>: Your drafts folder can be (re)organized to your liking. However, we recommend organizing them by file type (e.g. markdown or tei) as they are in this sample. You can choose to edit your transcriptions directly on GitHub in the drafts folder to create a version history, but this isn’t necessary! If you do, you will need to copy them over to the ready-to-publish items folder.

<span style="color: #63AEB6;">**source**</span>/<span style="color: #F7894E;">**drafts**</span>/<span style="color: #E44C31;">**markdown**</span>: blank sample files for each of the built-in genres (books, periodicals, and poems), which include all the hard-coded metadata fields ready for you to fill in.

<span style="color: #63AEB6;">**source**</span>/<span style="color: #F7894E;">**tei**</span>: your ready-to-publish TEI-encoded documents (.xml files).

<span style="color: #63AEB6;">**_texts**</span>: <span style="color: #E44C31;">**Markdown**</span> files that correspond to your <span style="color: #E44C31;">**TEI**</span> files.

<span style="color: #63AEB6;">**assets**</span>/<span style="color: #F7894E;">**images**</span>: home page banner image, site footer logos or marks, TEI-based page images

> <u>Note</u>: To replace the home page banner image with a custom banner image, follow the instructions under
<span style="color: #265095;">Configuring Your Edition Site</span> in Step 6.

<span style="color: #63AEB6;">**assets**</span>/<span style="color: #F7894E;">**images**</span>/<span style="color: #E44C31;">**tei**</span>: if you are using TEI and would like to include page images as part of your edition, add the image files to this folder.


Other folders beginning with an underscore (<span style="color: #63AEB6;">**_includes**</span>, <span style="color: #63AEB6;">**_layouts**</span>, etc.) contain files and code for the Jekyll site and theme.

### <u>**Step 6: Configuring Your Edition Site**</u>
The Recovery Hub template allows you to customize your edition by making changes (editing settings) in the <span style="color: #E44C31;">**_config.yml**</span> file. 

The <span style="color: #E44C31;">**_config.yml**</span> file contains settings that affect your whole site. <u>Listed below are the settings you will need to edit, along with instructions on how to modify</u> them for your edition site. You will only need to do this once; rarely will you need to make any edits afterward. 

#### **How do I Make Changes?**
Before we dive into customizing your edition site, you will need to know how to make changes in GitHub files. 

The following step-by-step instructions on making changes apply to <u>**all**</u> files in your GitHub repository. Since <span style="color: #265095;">Step 6</span> requires you to make changes in the <span style="color: #E44C31;">**_config.yml**</span> file to customize your edition, we felt it was only appropriate to use it in the steps below. 

Locate and open the file that you need to edit in your repository’s <span style="color: #265095;">main branch</span>: <span style="color: #E44C31;">**_config.yml**</span>

![Image 1](https://)
![Image Above: This is what you should see when you open the _config.yml file](https://)

Next, to make a change, switch to “edit” mode by clicking the pencil icon in the top-right corner of the file. You will not be able to make any changes if you are not in edit mode. 

![image](https://)

After you’ve made your changes, you can either “cancel” or “commit” to them. If you “cancel changes,” your edits will not be applied. Thus, unless you’ve changed your mind, you will choose “commit changes.”

![image](https://)

Before you can commit your changes, GitHub will present you with the option to keep the default or revise the commit message. This _**required**_ field serves as a brief, descriptive record of the changes made in a file. The Git commit message is a crucial part of version control, providing context and a history of code modifications for you and anyone else with access to the repository. Providing an “extended description” is _optional_. 

![image](https://)

Click “commit changes” to update your file.  

Now that you know how to make and commit changes to your files, let’s walk through how to update your settings in the <span style="color: #E44C31;">**_config.yml**</span> file to customize your edition site!

#### **Customizing Edition: Updating Settings in _config.yml** 
Locate and open the <span style="color: #E44C31;">**_config.yml**</span> file in the main branch of your edition’s repository.

Read through the file to familiarize yourself. **The lines starting with a #** indicate our detailed explanations of each setting and its function. Text after a # does not appear on the published site; we recommend keeping these lines to prevent confusion if you need to make changes later. 

You will add metadata to each element listed in the file, [see Fig. 7 below]:

![Figure 7: Metadata Element, “Title”](https://)

To edit and add your metadata, click the pencil icon in the top right corner and, from top to bottom, edit elements found under each section:

**Site Information Metadata**
- title
- URL and base URL: both must match your published site (see <span style="color: #265095;">Step 8</span> for instructions). 
- description

**Navigation Metadata**
- header pages

**Banner Metadata**
- banner image
- banner alt text
- banner size

Additional Site Information Metadata 
- editor
- contact information
    - name
    - email
    - institution
    - GitHub username
    - social media usernames (optional)

ADD MORE INFO HERE

Usually, you won’t need to change anything at the bottom of the file under “Other Settings.”

#### **Home Page Configuration**
To edit the home page of your site, you’ll need to edit the index.md and potentially make some changes in _config.yml, if you haven’t already. Instructions are provided in both files.

#### **About Page Configuration**
To edit the About page, make changes to the about.md file found in the main branch of your repository. If you don’t want to have an About page, delete that file instead.

#### **Adding New Pages**
You can add new pages to your site by creating new Markdown (.md) files. 

> Note: A page is a file. On your published site, the file functions as a web page.

To add a new page, click “Add file” in the top-right corner of your repository’s main branch, and click “Create a new file.” FINISH

![image](https://)

ADD MORE HERE

Note: A new page with additional information about your project can be stored in the main branch of your repository alongside <span style="color: #E44C31;">**index.md**</span> and <span style="color: #E44C31;">**about.md**</span>. If it’s a page about the texts in the edition, you may store it in your <span style="color: #63AEB6;">**paratext**</span> folder instead. 

### <u>**Step 7: Publishing your site with GitHub Pages**</u>
To publish your project edition site, click “Settings” at the top of your edition’s repository home page. This will direct you to the setting’s “General” page [Fig. #].

![image](https://)

Before you continue, **your _repository must be public_ before it can be published** with GitHub Pages. 

If your repository is already **public**, click <span style="color: #265095;">here</span> to jump ahead.  

If your repository is currently **private**, follow the steps below to make it public.

#### **Update Privacy Settings: Private to Public**
On the setting’s general page, scroll down till you reach “Danger Zone” and click “Change Visibility,” changing to public.

![image](https://)

Box 1 will appear [term for this box] and click “I want to make this repository public.”

Box 2 appear [term for this box] and click “I have read and understand these effects.”

Box 3 will appear [term for box] and click “Make this repository public.” 

![Box 1](https://)

![Box 2](https://)

![Box 3](https://)

After your repository has been made public, the page will reload and take you back to the top of the setting’s general page. Stay on this page and follow the directions below on how to publish your repository.

#### **Publish Project Edition**   

ADD SECTION

#### **Step 8: Change URL and Base URL**

ADD SECTION

### <u>**Additional Considerations**</u>

**Transcription & Editing**
<br>For detailed documentation on transcribing sources, organizing files, and preparing your edition for online publication, see our Markdown Transcription tutorial. 

If you plan to use TEI in your edition, you may also link directly to the TEI Guide.

**Troubleshooting**
<br>If you’re experiencing problems with your GitHub Pages site, the official GitHub Pages documentation has detailed troubleshooting information and is a good place to start.

