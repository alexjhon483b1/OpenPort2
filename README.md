grep -n "open" http.txt | awk -F: '{print $1+4}' | xargs -I {} sed -n '{}p' file.txt

grep -Eo '\b([0-9]{1,3}\.){3}[0-9]{1,3}\b' file.txt
