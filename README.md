![enter image description here](https://www.stardock.com/press/stardock%20branding/images/software/logo_strsof_fullcolor_full.png)
# Stardock-Software-Localization

 - [Mission](#mission)
 - [Supported Languages](#supported-languages)
 - [Editing and Submitting Languages](#editing-and-submitting-languages)
	 - [Creating a GitHub account](#creating-a-github-account)
	 - [Editing a language file](#editing-a-language-file)
- [Language File Format and Testing](#Language-File-Format-and-Testing)

## Mission
A public effort to improve language localizations for the Stardock software product catalog.

## Supported Languages
Stardock Software officially supports and maintains the following languages:
-   German
-   Spanish
-   French
-   Korean
-   Russian
-   Portuguese - Brazil
-   Chinese (Simplified)
-   Chinese (Traditional)
 
We will accept any other user-created languages, and include them in the products, but we will not officially maintain them.  Any updates for the non-supported languages will have to come from the community via this project.

## Editing and Submitting Languages
GitHub is the primary tool that Stardock uses to maintain our translations as it allows for streamlined contribution with a platform that is popular with many in our community. If you are familiar with this platform, you can skip to the [Language File Format and Testing](#language-file-format-and-testing) section to see how the language files are structured for each product, otherwise, onboarding directions are below.

The following directions are more for the laymen who want to contribute but do not want the complication of installing related software.
### Creating a GitHub account
The one thing you will need is a free [GitHub account](https://github.com/join). 

### Editing a current language file
In this example, we will:
 - Initiate editing an existing DeskScapes language file
 - Creating a fork \ branch to edit it under your credentials
 - Creating a 'pull request' to have it reviewed and included in the main repository

Click on the /Apps/DeskScapes/DeskScapes 11 folder and select a language you wish to edit
![enter image description here](https://cdn.stardock.us/support/uploads/msedge_2024-01-19_12-10-18.png)

Click the edit pencil 
![enter image description here](https://cdn.stardock.us/support/uploads/Teams_2023-10-02_13-24-45sdrohan.png)

You will be notified that to edit the file, it needs to be 'forked' to continue.  Forking any file is just an act to create a copy under your own account.
![enter image description here](https://cdn.stardock.us/support/uploads/Teams_2023-10-02_13-28-54sdrohan.png)

You can now freely edit the file under your own forked copy.  Once done, click the green 'commit changes' button

### Commiting a new or edited language file
In the commit popup, add some details about what you added or changed and why (poorly phrased, inaccurate word choices, etc.). Click 'propose changes' once done:
![enter image description here](https://cdn.stardock.us/support/uploads/Teams_2023-10-02_13-32-02sdrohan.png)

After you have edited one or more files, create a 'Pull request' (you are asking us to 'pull' your changes from your fork with this act)
![enter image description here](https://cdn.stardock.us/support/uploads/Teams_2023-10-02_13-34-18sdrohan.png)

As you did for the individual files, you can write more details about any changes you made
![enter image description here](https://cdn.stardock.us/support/uploads/Teams_2023-10-02_13-36-21sdrohan.png)

When complete, we are automatically notified. Once reviewed, we will communicate with you (via GitHub and its email notification system) if we have any questions and either accept or deny the pull. If accepted, you will be credited in the changelog for any application release. 

### Adding a new language file
The en (English) file can be used as a template for all new language files.  

On your local PC, in the directory where the lang file is stored, copy the en.lng file and immediately paste it in the same directory - creating a 'copy' of it.  Rename it to the [ISO 639-1 Cod](https://www.loc.gov/standards/iso639-2/php/code_list.php) formatted lng file (example de.lng for German)


Open it, copy all the text, and use the 'Add file' option to create a new file in your fork, pasting in the English text for editing. 
![Add file](https://cdn.stardock.us/support/uploads/msedge_2023-10-04_11-12-09.png)

## Language File Format and Testing
### App group A

 - Start11
 - Groupy
 - DeskScapes
 - Multiplicity

#### Group A File format
The en.lng file is the base for which all other language files are generated. 

The only section that should be edited is under the [Strings] block and leaving the 'Exists=1' to start it.
>[Strings]
>Exist = 1

English (en) file example:

> "Which theme do you want to use?"="Which theme do you want to use?"

Spanish (es) file example:

> "Which theme do you want to use?"="¿Qué tema quieres usar?"

The ; (semi-colon) is used for comments in the file and anything following it will not be read by the app.

### Testing Language Files
After you have edited a language file, you should download it from your fork and put it in the app folder so it can seen to fit in the UI.

For example, this would be a translation that would be rejected as the translated text exceeds the UI's space for it.
![enter image description here](https://cdn.stardock.us/support/uploads/msedge_2023-10-02_16-04-45.png)

Language files for Group A products are stored in:
C:\Program Files (x86)\Stardock\[appName]\lang

For example, Groupy's language files are located in:
C:\Program Files (x86)\Stardock\Groupy2\lang

### App group B


 - Fences
 
 Coming soon
