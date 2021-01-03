# Linux Sed Command

stands for stream editor, which is used to search a word in the file and replace it with word required to be in the output. 

Note: it will only modify the output, but there will be no change in the original file. 

Examples:

## Update output hi to hello
``
sed 's/old_text/new_text/' file_name
``
## Update output hi or (hi)ght to hello (g for global)
``
sed 's/old_text/new_text/g' file_name
``
## Update  hi to hello in file
``
sed -i 's/old_text/new_text/' file_name
``
## A way to select parts of file instead of tail and head 
``
sed -n '5,10p' file_name
sed '10,20d' file_name
``
