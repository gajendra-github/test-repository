
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

  
  
  
  
  
  
  
  
