# Assignment-2
# Task 1: Repository Initialization

* Create a new Git repository
* Initialize the repository with the following branches:
    * `main`
    * `develop`
    * `feature/login`
     * <img width="1145" height="729" alt="Screenshot_20260419_174721" src="https://github.com/user-attachments/assets/4b738805-aac2-49c6-94ed-d03345cfd560" />




 # Task 2: Branching Workflow

* Create 2 feature branches (feature/payment, feature/profile)
    * 1 bugfix branch (bugfix/login-error)
    ```
        git checkout -b feature/payment
        git checkout -b feature/profile
        git checkout -b bugfix/login-error
    ```
    * <img width="846" height="267" alt="Screenshot_20260419_175344" src="https://github.com/user-attachments/assets/777953b3-75a8-436f-8e87-9b90ad952776" />


* Perform:
   * code change and commit feature/payment, feature/profile, bugfix/login-error
  *   <img width="1081" height="685" alt="Screenshot_20260419_181504" src="https://github.com/user-attachments/assets/1b761628-aec0-4e2f-abcb-c22a9216aec6" />


   * **Merge Strategy** - Merge bugfix/login-error branch into main branch
   * <img width="718" height="185" alt="Screenshot_20260419_181826" src="https://github.com/user-attachments/assets/6500c5c9-27e3-48b1-99bd-9c6465a9181d" />


   * **Rebase Strategy** - We will integrate feature/profile using a rebase.This moves the branch's history to the tip of main for a linear timeline.
   * After rebasing, feature/profile merging it into main
   * <img width="724" height="405" alt="Screenshot_20260419_182052" src="https://github.com/user-attachments/assets/7676d9de-0061-4a8f-bcbc-9daa3284bc4e" />
# Task 3: Commit History Management
   * * In feature/payment :
  * Make at 5 commits
  * 
  * <img width="751" height="565" alt="Screenshot_20260419_202646" src="https://github.com/user-attachments/assets/9cf9c1cd-28e0-4ad6-9937-29315e961e48" />


   * Combine commits using *Reword*
   * typing this command "git rebase -i HEAD~5".. a new text editor pop up like this
   ```
pick a1b2c3d change file 1
pick e5f6g7h change file 2
pick i9j0k1l change file 3
pick m2n3o4p change file 4
pick q5r6s7t change file 5
```
   * Reword: Change the first pick to reword (or r). This lets you change the message of the "base" commit.
   * A second window will pop up asking for the new commit message (because of the reword command).
     * Type a clean message like "Change The File Number 1" and save.
       
   * <img width="743" height="734" alt="Screenshot_20260419_195433" src="https://github.com/user-attachments/assets/c473c311-d4c1-4cfd-b214-77404d047ac7" />


* Combine commits using *Squash*:
   * as like same type  "git rebase -i HEAD~5"   when the text editor pop up without first commit all pick alter with squash.
   * Squash: Change the next four pick entries to squash (or s). This melts those changes into the first commit.

```
pick a1b2c3d Change The File Number 1 
squash e5f6g7h change file 2
squash i9j0k1l change file 3
squash m2n3o4p change file 4
squash q5r6s7t change file 5
```

* <img width="747" height="726" alt="Screenshot_20260419_200640" src="https://github.com/user-attachments/assets/dc794dfa-1a43-4cef-b8ea-146eb891c6d9" />

* Result: 5 messy  commits are now one single, clean commit with a professional message.
* here the last git log
* <img width="719" height="167" alt="Screenshot_20260419_201034" src="https://github.com/user-attachments/assets/cd720790-a209-421e-abef-9fc384090c5f" />
