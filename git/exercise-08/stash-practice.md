# What I Did Today: `git stash`

Today, I learned how to use the `git stash` command.

The `git stash` command is used to temporarily save changes in your working directory without creating a 
commit. This is useful when you're not ready to commit your work but need to switch tasks or branches.

Here's how I tested it today:

* I opened a file that had already been committed before, `notes.txt`.
* I added a new line: "New line of text in the `notes.txt` file".
* I ran `git status` to confirm that the file had been modified.
* Then, I used `git stash` to temporarily save my changes.
* After that, I ran `git stash show` to verify that the stash had been created.
* I checked the contents of `notes.txt`, and as expected, my changes were no longer there.
* Finally, I restored the changes using `git stash pop` and confirmed that the new line was back in `notes.txt`.

# When Would I Use `git stash`?

One situation where I would use `git stash` is when I need to switch to another branch, but my current 
changes aren't ready to be committed yet. Instead of creating a temporary commit, I can stash my changes, 
switch branches, and later restore them with `git stash pop`.
