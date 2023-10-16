# Alfred-workflow-move-folder
Move folder with option to merge files to identically named existing folder

# WARNING

One option in this workflow allows you to merge two identically named folders (which is the default in the workflow configuration).  *Before you use that function for the first time please backup your original folder and any identically named folder located in the destination so that you can check, without risk of losing data, that the function works as you expect.*

# Introduction

Select a single folder in Finder, activate Alfred using your Universal Action hotkey then use this workflow to move that folder and its files to a destination of your choice. If an identically named folder exists in the destination you will be offered the options of either overwriting that folder or of merging the contents of both folders. The latter option produces a folder in the destination containing both the files from the original folder (which will be moved to the Bin/Trash) *and* the files that were already in the identically named folder.

# Configuration

When there is an identically named folder in the destination you will have the option of either overwriting the identically named folder or of merging the files from the two folders.

The workflow configuration allows you to choose which option appears as the default in the relevant dialog (see workflow Read Me).

The options available are the same but the default dialog choice (which you can select by pressing ⏎) changes. The purpose of the configuration is to allow you to have your most-used function as the easily accessible default.

# Usage

Select a single folder in Finder, activate Alfred using your Universal Action hotkey and find the workflow by starting to type `Move folder`. After pressing ⏎ you will be prompted for the name of the destination. Start typing the folder name and select the folder you want.

If an identically named folder does not exist in the destination the selected folder will simply be moved to the destination.

If, however. an identically named folder does exist you will see one of two dialogs (see `Configuration` above). Which you see will depend upon whether or not the checkbox in the configuration is checked.

If you choose to merge the files they will be merged in the destination and the original folder will be moved to the Bin/Trash.

If you choose to overwrite the existing folder the moved folder and its contents will replace the identically named folder in the chosen destination.

# Creation of log file on merge

When you choose to merge two identically named folders a log file (called `mergelog.txt`) is created in the workflow's home folder. To see it right click on the workflow name in Alfred's preferences and choose `Open in Finder`. You can then open the `mergelog.txt` file in your default text editor to see exactly what changes were made during the merging of the folders.

*Note that the log file is overwritten by each fresh merge to prevent it becoming unwieldy.*
