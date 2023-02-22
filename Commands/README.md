# Areas
![areas](https://user-images.githubusercontent.com/99830416/220210277-b4fc9d57-462a-463c-88d9-893c89c7b0f8.jpg)

![separator2](https://i.imgur.com/4gX5WFr.png)

# From Local To Remote 

### `git status`
-  Return information of your **Local Repo**

### `git add [file name or folder name or *] `
- Add the selected files to be in **Staging area**
- \* add all untracked files into Staging area

### `git reset head [file path or folder name]`
- Unstage tracked (staged) file. Remove this file from staging area

### `git commit -m "message"`
- Move files from staging area to **Local repo**

### `git branch`
- List all branches you have and the current branch wiht * sign  

### `git remote`
- Return RemoteName 

### `git push [RemoteName][BranchName]`
- `git push origin main  //main is default local branch`  

- `git push origin Gaber //Gaber is a local branch`  

![separator2](https://i.imgur.com/4gX5WFr.png)

# From Remote To Local

### `git pull origin`
- Get all edited files in remote repo to local
- Do 2 commands : git fetch [retrieve  data from remote] , git merge [merge those data to your local branch]

![separator2](https://i.imgur.com/4gX5WFr.png)

# Pull and push 

### `git push -u origin [BranshName]`
- Pull then push

![separator2](https://i.imgur.com/4gX5WFr.png)


# Configurations

## ListConfigurations
### `git config -l`
- return your configurations


## Editor
### `git config --global core.editor code`
- Set vs code as your default editor

### `git config --global --edit`
- Open configurations on vs code
- You can set your configurations using vs code
  
  ![image](https://user-images.githubusercontent.com/99830416/220574337-200a275e-b10a-4830-866c-ed1c6c244b06.png)


## UserName & UserEmail
### `git config --global user.email`
- Return user email

### `git config --global user.email "email"`
- Set your email

### `git config --global user.name`
### `git config --global user.name "name"`
- Get and set user name

## Alies
### `git config --global alias.pl pull`
- Set config

### `git config --global alias.pl`
- Get the value of alias


## UnsetConfig
### `git config --global --unset configname`
- unset specific configuration : user.name, user.email and so on


 
![separator2](https://i.imgur.com/4gX5WFr.png)
# Pull Request

![separator2](https://i.imgur.com/4gX5WFr.png)

# Branching

## Create branches and move between them
### `git branch`
- return all branches in repo 
- \* sign to the current branch

### `git branch branch_name`
- Create branch with branch_name

### `git checkout branch_name`
- Travel between branches

### `git checkout -b branch_name`
- Create the branch and travel to it

### `git branch -m new_branch_name`
- Rename the current branch


## Delete Branch
`Note to travel to another branch to be able to delete the branch`

### `git branch -d branch_name`
- Safe mood
- Git checks if the branch has changes that not merged yet to the master branch if (true) it will be not deleted else delete

### `git branch -D branch_name`
- Force mood
- Delete the branch without checking


## Merge Branch in git 

### `git checkout main` `git merge branch_name`
- Merge main branch with another branch

## Send branch to githup 
### `git push origin branch_name`
- Sent to gihhup and we can merge there


![separator2](https://i.imgur.com/4gX5WFr.png)


# Stash
## Usage 
Used to stash [Hide] some commits that you do not want to commit now. Same mexanism of stack [Last In First Out LIFO]

### `git stash`
- Hide files that added to staging area 

### `git stash save "message"` 
- add message to your stash 

### `git stash list`
- List stash array 

![image](https://user-images.githubusercontent.com/99830416/220619724-c0be96af-b6f5-40da-aa59-87a0425145bc.png)


### `git stash pop`
- Return last elements added to stash ( stash[0] ) and pop it [stash.top() then stash.pop()] 





![separator2](https://i.imgur.com/4gX5WFr.png)
