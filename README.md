# `anonymizer` extension for TYPO3

## What does it do?

This extension add possibilities to anonymize selected data in public area. You can use it i.e. for:

- Showing your application to public audience during demonstration to client, on conferences, trainings, webinars, etc.
- Building application that will be used in public area, like info/consulting points, to prevent possibility of displaying real data like phone numbers or emails to bystanders.
- Anonymizing your API endpoints for 3-rd party data analyzing tools.
- Permanent anonymizing your database tables for sharing its parts or even whole databases with 3-rd party co-developers.

## `for-developers-only`

This extension delivers several classes and view helpers, that allows the developers to fasten their work during developing custom TYPO3 extensions, if you don't know what is that all mean, and you don't want to know, fell free to abandon further lecture. Otherwise, you're kindly welcome to process.


## Will my original data be changed?

Shortly: NO. 

In more details: this extension DOES NOT modify data in tables you are anonymizing, instead creates cached version of selected tables and/or fields, so after switching anonymizer off you'll have your original values available back without need of re-anynomizing.

**Warning! This step MAY BE DESTRUCTIVE for your instance**

If you need to anonymize tables permanently, i.e. to share with 3-rd party developers you need to do it yourself, operating directly on database. Remember that permanent anonymizing tables like `fe_users` or `be_users` may cause problems with login to frontend or backend, or other unexpected errors. 

[_Missing documentation: This part will be described with samples in official documentation later in the time._] 

## Current version

`0.5.0 alpha`

#### Unstable version

Until this extension's version is in unstable version like `alpha` or `beta` you shouldn't use it in ANY production environment. Please wait for `stable` state, also feel free to contribute to make it `stable` faster and better. We are happy to see you at our team!

## Contributors wanted!

To become a contributor, please first create an issue at https://github.com/biesior/anonymizer/issues.

After that, please wait for our response, before you'll start to code. Keep in mind, although we're opened to any suggestions, not every one can be incorporated into `master` branch at this moment. Maybe it requires discussion, clarification and/or verification, or maybe your concept will never go to the repository. For sure, we'll try to answer every request that is sent.  

We'll apreaciate any kind of contribution, especially in role(s) of:

- Team leaders  
  anybode who's able to keep the project in the order
- Developers  
  anybody who has the skills to develop the code
- Testers
    - Manual  
      anybody to click and check if everything is working as expected
    - Automatic  
      anybody who can write automatic tests for PHP Unit
- Documentation writers  
  anybody who wants to write RST documentation

## TYPO3 Helpers by 99° tribute

This extension uses some selected parts of code and ideas extracted from [TYPO3 Helpers by 99°](https://extensions.typo3.org/extension/nnhelpers) extension delivered to you by [99° + Lindner & Steffen](https://www.99grad.de). If you are an ambitious developer, consider using their extension to drastically speed up your extension development and don't forget to send your paid support for coffee for Minions.

Check yourself:

[TYPO3 Helpers by 99° in TYPO3 extensions repository](https://extensions.typo3.org/extension/nnhelpers)  
[TYPO3 Helpers by 99° external manual](https://labor.99grad.de/typo3-docs/nnhelpers/de/)

### TYPO3 Helpers by 99° description

Drastically speed up your extension development with this huge collection of very smart 'oneliners'. Make updating to new TYPO3 versions simple. Packed with things you've spent hours searching on the internet for. Everything accessible with one click via a convenient backend module. No mess and no conflicts. Use whatever method makes you happy – or simple grab the source-code and paste it in your own extension.
