# note-system
A collection of scripts that I use in conjunction with flashbake for my personal notetaking system

I like making Git do nifty things for me. One of those things is tracking my personal working notes. 

I use a simple system of organization for notes. Every day, I create a new file titled mm-dd-notes (where mm is the month and dd is the day). Those files are organized in a flat-file system by year and month (e.g., my notes for the 23rd of November live in ~/Notes/2015/11/11-15-notes). 

Thanks to Thomas Gideon and the [Flashbake tool](https://github.com/commandline/flashbake/), I can automatically commit changes to my notes in a git repository using a cronjob. With the addition of the two scripts in this repo, I can simplify how I create and access my notes, as well as automatically sync changes to a remote git repository. 

To use this tool as your very own:

1. Set up a git repo for your notes.
2. [Install Flashbake.](https://github.com/commandline/flashbake/wiki/Installation)
3. Create an SSH key specifically for your Notes repo.
4. Pull this repo and edit the `# SETTINGS !` section to meet your needs
5. Add both scripts to your $PATH. (I prefer ~/.bin)
6. Add `notes-sync` to your crontab. (5 minutes seems to be adequate, but YMMV.)

And that's it. Enjoy!


### Release Notes

v0.1, 23 November 2015: initial release.


