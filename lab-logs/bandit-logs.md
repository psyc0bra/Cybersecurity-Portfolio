# 📂 Level-by-Level Command Log

### Levels 0 -> 3: The Basics of Navigation
* **Level 0:** Used `ssh` to establish a secure connection to the remote lab.
* **Level 1:** Conquered the "dashed" filename. Used `cat ./-` to tell Linux that `-` was a file path, not a command flag.
* **Level 2:** Handled spaces in filenames. Used `cat "spaces in this filename"` to keep the name together.
* **Level 3:** Found hidden data. Used `ls -a` to reveal the "dot" files that were invisible to a normal search.

### Levels 4 -> 6: The Digital Bloodhound
* **Level 4:** Used the `file` command on everything in the directory (`file ./*`) to find the one human-readable text file among binary junk.
* **Level 5:** Used `find . -size 1033c` to instantly locate a file based on its exact weight in bytes across dozens of folders.
* **Level 6:** The "Deep Search." Used `find / -user bandit7 -group bandit6 -size 33c 2>/dev/null` to scan the entire server while muting "Permission Denied" errors.

### Levels 7 -> 10: Data Analysis & Decoding
* **Level 7:** Used `grep millionth data.txt` to pull a single password out of a massive wall of text.
* **Level 8:** Mastered de-duplication. Used `sort data.txt | uniq -u` to find the one unique line that wasn't repeated.
* **Level 9:** Gained "X-Ray Vision." Used `strings data.txt | grep "=="` to find a password hidden inside a binary (non-text) file.
* **Level 10:** Dealt with web-data encoding. Used `base64 -d data.txt` to turn gibberish into a clear, usable password.

### Levels 11 -> 13: Cryptography & Remote Access
* **Level 11:** Deciphered the **ROT13 cipher**. Used `tr 'A-Za-z' 'N-ZA-Mn-za-m'` to "rotate" the alphabet by 13 positions, mapping the scrambled text back to the original password.
* **Level 12:** The **"Hex Dump" puzzle**. Used `xxd -r data.txt` to convert a hex dump back into binary, then iteratively used `file`, `zcat`, `bzip2`, and `tar` to peel back multiple layers of nested compression like a digital Russian nesting doll.
* **Level 13:** The **Private Key Pivot**. Encountered a "localhost login blocked" error. Solved it by using `scp` to download the `sshkey.private` file, applying `chmod 600` to satisfy SSH security requirements, and authenticating directly from my local terminal using the `-i` flag.
