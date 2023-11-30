# Lab 4
![Step 4](step4.PNG)\
The keys pressed for this command were `ssh cs15lfa23gt@ieng6.ucsd.edu<enter>`. This command was used to log me in to the ieng6 server.\
![Step 5](step5.png)\
The keys pressed for this command were `git clone <ctrl+v><enter>`. This command clones the repository, where `git@github.com:srajendra001/lab7.git` was what was copied from the clipboard.\
![Step 6](step6.PNG)\
The keys pressed for this command were `bash t<tab><enter>`, which ran the tests. Using the `<tab>` button autocompleted the t character to `test.sh`.\
![Step 7](step7.PNG)\
The keys pressed for this set of commands were `vim L<tab>.<tab><enter>`, `?index1<enter>`, and `er2:wq<enter>`. The first command opened the `ListExamples.java` file in vim. The second command searched for the last instance of `index1`, which happened to be the one that needed to be changed. This put the cursor at the first character of the last `index1`. The next step moved the cursor to the last character in `index1`  and replaced it with a 2 to fix the error. Finally the file was saved and vim was exited.\
![Step 8](step8.PNG)\
The keys pressed for this command were `<up><up><enter>`. Doing this finds the bash history 2 lines up, which was `bash test.sh`, and runs the tests.\
![Step 9](step9.PNG)\
The keys pressed for this set of commands were `git status<enter>`, `git add <tab><enter>`, `git commit<enter>`, `<shift+g>i<del>Fixed ListExamples.java to have correct output<esc>:wq<enter>`, and `git push <enter>`. First, the current status was checked. Then, the `ListExamples.java` file was staged to be committed. It was committed using vim to create a special commit message for GitHub. Finally, the commit was pushed to the remote repository to reflect the changes made on the local computer.
