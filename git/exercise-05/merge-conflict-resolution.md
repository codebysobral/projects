# How I resolved a branch conflict

*1. Creating a conflict* 
My main branch was main. I created a second 
branch named feature-conflict from 
main and switched to it using git 
switch feature-conflict. I created a 
file named simples.txt containing 
the text "A simple title" on the 
first line, saved it, and committed 
the changes.

Then, I switched back to main, 
created the same file simples.txt, 
but with the text "A complexity 
title" on the first line, saved it, 
and committed the changes.

*2. Starting a merge* 
After creating the conflict, I 
initiated the merge by running git 
merge feature-conflict while on the 
main branch and encountered a merge 
conflict.

*3. Observing the conflict* 
For conflict-free merges, the message that 
appears is simply "Fast-forward." 
However, for merges with conflicts, Git 
displays a message like "CONFLICT 
(content): Merge conflict in 
<file-name>"—and that was the message 
that appeared.

*4. resolving the conflict* 
I opened the file where I had made different 
changes in the two branches and noticed 
that Git was showing the differences 
between the two versions. I then made 
the final changes, ran the git commit 
command, and the conflict was resolved.

*5. Observing the result* 
After the merge was successfully completed, I 
checked the merge history using git log 
--oneline --graph and got the following 
result:

*   603f1a6 (HEAD -> master) Merge branch 'feature-conflito'
|\
| * f971dab (feature-conflito) Conflict Version!
* | afd62f7 Version of Marters
* | 16fa66d Master Version
|/
* f68ec0d (feature-simples) Altera
* 359ea6e Mensagem correta
* 4f7e4d5 Add new line
* 347772b docs: add notas file
* 8835c15 Add notes.txt
