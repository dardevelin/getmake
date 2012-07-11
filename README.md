#getmake 
getmake is a small group of poorly set bash scripts
to facilitate makefile and Cmakefile integration with projects

## SETTING UP
most linux distribuitions have a .bashrc file in the user
home directory, if yours doesn't you will need to make your own
some distros like debian use that file for some configurations
if you don't want to mix your alias with the distros ones, look at
bashrc in this repository it shows what you need there so you can 
do your alias in a seperate .bash_aliases file

either way the alias you need to include in your file are all in
.bash_aliases in this repository

your template code should live in a your home directory /Templates/code
later versions will allow automatic install and configuraton for now
if you want changes you need to manually edit the .sh files

make a directory in home directory:
    mkdir .getmake

add the following list of files in there
 - getmake.sh
 - getmake-ls.sh
 - getmake-add.sh
 - getmake-rm.sh
 - getmake-cat.sh
 - getmake-edit.sh

now you need to give them permission so they can run properly

chmod +x getmak*

and now should all be set, when you open new terminals 
all should be working


###quick tour
getmake-ls           | lists your templates
getmake-cat filename | shows the contents of filename in templates
getmake-add file_to_add template_name |
getmake-rm  filename | removes filename from templates
getmake-edit "editor and flags" filename

