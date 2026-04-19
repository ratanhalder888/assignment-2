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
