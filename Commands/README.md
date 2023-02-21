# Areas
![areas](https://user-images.githubusercontent.com/99830416/220210277-b4fc9d57-462a-463c-88d9-893c89c7b0f8.jpg)

![separator2](https://i.imgur.com/4gX5WFr.png)

# From Local To Remote 

### `git status`
-  Return information of your **Local Repo**

### `git add [file name or folder name or *] `
- Add the selected files to be in **Staging ares**
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
- Set your configurations using vs code 


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

![separator2](https://i.imgur.com/4gX5WFr.png)

