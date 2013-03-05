Red Theme for Alfresco Share
============================

Author: Will Abson

This project defines an additional theme for Alfresco Share using a red 
colour scheme.

Installation
------------

The theme has been developed to install on top of an existing Alfresco 3.3 
installation.

An Ant build script is provided to build a ZIP file containing the 
custom files, which can then be installed into the 'tomcat' folder of your
Alfresco installation.

To build the ZIP file, run the following command from the base project 
directory.

    ant dist-zip-tomcat
    
The command should build a ZIP file named redTheme.zip in the 'dist' directory 
within your project.

Once you have run this you will need to refresh the list of web scripts in 
Alfresco Share using the page at http://localhost:8080/share/page/index, in 
order to pick up the new theme. An optional Ant task reload-webscripts-webtier 
is provided commented out in the build script if you wish to use this.

Selecting the theme
-------------------

Log in to Alfresco Share as a repository administrator and click the Admin
Console link. In the Application section select 'Red Theme' from the Theme
drop-down list and confirm your changes.

The theme will now be used for all users as the application default.