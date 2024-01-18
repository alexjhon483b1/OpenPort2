you are interested in 4 lines before the line that contains the word open
grep -n "open" file.txt | awk -F: '{print $1+4}' | xargs -I {} sed -n '{}p' file.txt

grep -Eo '\b([0-9]{1,3}\.){3}[0-9]{1,3}\b' file.txt
