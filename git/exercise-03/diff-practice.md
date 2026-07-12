#Practical git diff commands

*1. Starting in the test repository*
To start, I entered my test
repository, opened `notes.txt` using the `nano` command, and added
another line of text.

*2. Using the git diff command*
After adding a new line to my `notes.txt`
file, I ran the `git diff notes.txt` command and observed the changes in
the text, indicated by the plus (`+`) symbol.

*3. Using git `diff --staged`*
After noticing changes in the working tree using the `git diff <file>`
command, I decided to move the file to the staging area and use the `git
diff --staged notes.txt` command to verify that the changes were no
longer shown in the working tree, but instead in the staging area.

*4. Restoring the file with `git restore`.*
After modifying my `notes.txt` file again and saving it, but before adding
it to the staging area, I decided to restore the previous version
using `git restore notes.txt`.

*5. Moving the file from the staging area to the working directory*
After modifying the `notes.txt` file again, I added it to the staging
area using `git add notes.txt`. However, I decided to make another
change, so I needed to unstage the file and move it back to the working
tree. To do this, I used the command `git restore --staged notes.txt`.

*6. Renaming a commit*
I made a test commit using `git commit -m "test commit"`, but decided to
rename it to "add notes". So, I used `git commit --amend -m "add
notes"`.

*7. Using .gitignore*
I used a `.gitignore` file to exclude files I didn't
want to push to the online repository. I created the `.gitignore` file
using `touch .gitignore` and then edited it with `nano .gitignore`,
listing all the files I wanted to exclude. To test this, I created a
file named `debug.txt` and configured `.gitignore` to ignore all files
with the `.txt` extension using the pattern `*.txt`. However, even
though I was ignoring all `.txt` files, I still wanted `notes.txt` to be
included in the online repository, so I added `!notes.txt` to create an
exception to the previous rule.
