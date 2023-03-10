
#### README.markdown  
- default name that is given to the documentation but can use any other name for documentation file as long as it adheres to markdown language syntax


##### Configure git on local computer  (These details will be associated with any commits that you create)
 $ git config --global user.name "username"
 
 $ git config --global user.email "useremail@test.com" (should match with signup email)
 
 
 
 
##### Copy code from remote (github) to local computer
  $ git clone https://github.com/gajendra-github/test-repository.git
  
  
  $ git status
  
  $ git diff README.md
  
  $ git add README.md      (staged .... ready for commit)
  
  $ git commit -m "updated the readme file" 
  
  $ git log --oneline       (to check the status of local and remote commit)
  
  (HEAD -> main) Updated readme file : local computer is at this commit.
  
  (origin/main, origin/HEAD) Initial commit : remote (github) is at this commit.
  
  $ git push origin main    (new repository called main)
  
  $ git push origin master  (old repository called master)
  
  ##### possible error message after username/password:
  remote: Invalid username or password.
  
  fatal: Authentication failed for 'https:github.com/test-repository.git'
  
  ##### OR
  remote: Support for password authentication was removed on August 13, 2021 
 
  remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on 
          currently recommended modes of authentication.
  
  fatal:  Authentication failed for 'https://github.com/test-repository.git'

  #### Solution
  Support for password authentication was removed on August 13, 2021
  
  In order to fix the issue follwo below steps:
  
  1. Goto settings of Github account
  2. Find and Select Developer Settings
  3. Find and Select Personal access tokens
  4. Generate a new token
  5. Fill in any note and select the access scopes
  6. Once done click generate token
  7. Use the generated token in place of a password to communicate with GitHub.


  
  
  #### possible success message after git push origin master
  Enumerating objects: 5, done.
  
  Counting objects: 100% (5/5), done.
  
  Delta compression using up to 8 threads.
  
  Writing objects: 100% (3/3), 321 bytes | 321.00 KiB/s, done
  
  Total 3 (delta 1), reused 0 (delta 0)
  
  remote: Resolving deltas: 100% (1/1), completed with 1 local object. 
  
  To github.com: Username/test-repository.git
  87e4873939..7agd main -> main
  
  
  $ git push origin master
  
  #### possible error message if local and remote work won't match.
  
  ! [rejected]  main -> main (fetch first)
  
  error: failed to push some refs to 'https://github.com/username/test-repository.git'
  
  hint: updates were rejected because the remote contains work that you do not have locally. This is usually caused by another repository pushing
        to the same ref. You may want to first integrate the remote changes (e.g., 'git pull ...') before pushing again. See the 'Note about fast-             forwards' in git push --help' for details.
        
        
        
#### git init
Using master as the name for the initial branch. This branch name is subject to change. To configure the initial branch name to use in all
of your new repo , which will supress this warning call...

git config --global init.defaultBRanch <name>

Names commonly choosen instead of 'master' are 'main', 'development' . The just created branch can be renamed via this command

$ git branch -m <name>







  
  
  
  
  
  
  
  
  
