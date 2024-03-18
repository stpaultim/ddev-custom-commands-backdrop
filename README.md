# ddev-custom-commands-backdrop
Some custom commands for using DDEV with Backdrop CMS

This is code to customize DDev specifically for Backdrop CMS development. Adding some custom configuration
that I used to use with Lando and wanted to replicate with DDev. 

To start with, it's simple commands to create a snapshot of files directory and database that can easily 
be reverted to. For my initial draft, I'm assuming that config files are stored in files directory and 
get managed as part of the files directory. 

In the future, I'd like to treat them seperately, in case they are not stored in files directory. But, that
might be left to be handled on a case by case basis.

Currently, this package only includes two commands. The custom command files need to be placed in the 
following directory. 

- .ddev/commands/web/*

Once these commands are in place, you should restart the ddev environment and you will be able to use
these commands:

* ddev snapshot
* ddev reset

Pull requests are welcome. I know that the code could be improved quite a bit and I welcome assistance.
