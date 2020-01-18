# cdb
Bookmark tool for command line navigation.

## Setup

```
RCFILE='.bashrc' # Or .bash_file for Macs
cd ~ # directory where you want to keep cdb
curl -O https://raw.githubusercontent.com/cpagravel/cdb/master/cdb
echo "source $PWD/cdb" >> ~/$RCFILE
```

## Usage
```
cdb # display list of bookmarks
cdb <int> # navigate to bookmark on list
cdb -d <int> #  delete a bookmark
mark # add current directory to list of bookmarks
```

## Examples
```
## Create bookmark
$ cd ~/Documents
$ mark # create bookmark here
$ cdb # list bookmarks
1. Documents        /home/cpagravel/Documents

## Navigate to a bookmark
$ cd ~
$ pwd
/home/cpagravel
$ cdb 1 # navigate to bookmark 1
$ pwd
/home/cpagravel/Documents

## Delete a bookmark
$ cdb -d 1 # delete bookmark 1
$ cdb # list bookmarks
# Nothin will display
```
