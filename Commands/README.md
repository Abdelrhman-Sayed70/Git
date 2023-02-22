# ⦿ Areas
![Picture1](https://user-images.githubusercontent.com/99830416/220769928-aada5303-11cb-4de1-93ca-4a4613e59b50.jpg)
![separator2](https://i.imgur.com/4gX5WFr.png)



# ⦿ Local ⭢ Remote 
> ### `git status`
> -  Return information of your **Local Repo**
> 
> ### `git add [file name or folder name or *] `
> - Add the selected files to be in **Staging area**
> - \* add all untracked files into Staging area
> 
> ### `git reset head [file path or folder name]`
> - Unstage tracked (staged) file. Remove this file from staging area
> 
> ### `git commit -m "message"`
> - Move files from staging area to **Local repo**
> 
> ### `git branch`
> - List all branches you have and the current branch wiht * sign  
> 
> ### `git remote`
> - Return RemoteName 
> 
> ### `git push [RemoteName][BranchName]`
> - `git push origin main  //main is default local branch`  
> 
> - `git push origin Gaber //Gaber is a local branch`  
>
![separator2](https://i.imgur.com/4gX5WFr.png)




# ⦿ Remote ⭢ Local
> ### `git pull origin`
> - Get all edited files in remote repo to local
> - Do 2 commands : git fetch [retrieve  data from remote] , git merge [merge those data to your local branch]
> 
![separator2](https://i.imgur.com/4gX5WFr.png)





# ⦿ Pull and push 
> ### `git push -u origin [BranshName]`
> - Pull then push 
> 
![separator2](https://i.imgur.com/4gX5WFr.png)






# ⦿ Configurations
## ListConfigurations
> ### `git config -l`
> - return your configurations

## Editor
> ### `git config --global core.editor code`
> - Set vs code as your default editor
> 
> ### `git config --global --edit`
> - Open configurations on vs code
> - You can set your configurations using vs code
>   
>   ![image](https://user-images.githubusercontent.com/99830416/220574337-200a275e-b10a-4830-866c-ed1c6c244b06.png)

## UserName & UserEmail
> ### `git config --global user.email`
> - Return user email
> 
> ### `git config --global user.email "email"`
> - Set your email
> 
> ### `git config --global user.name`
> ### `git config --global user.name "name"`
> - Get and set user name

## Alies
> ### `git config --global alias.pl pull`
> - Set config
> 
> ### `git config --global alias.pl`
> - Get the value of alias

## UnsetConfig
> ### `git config --global --unset configname`
> - unset specific configuration : user.name, user.email and so on

![separator2](https://i.imgur.com/4gX5WFr.png)






# ⦿ Pull Request

> - Check if the repo owner put rules to contribute 
> - Fork Repo you want to contribute on it
> - Make your changes on your forked local repo 
> - Go to your forked repo on githup and create pull request
> 
>   ![image](https://user-images.githubusercontent.com/99830416/220724964-749653c5-49bd-4ab2-9273-f103677b6eef.png)
>   
>   ![image](https://user-images.githubusercontent.com/99830416/220725231-b05976c4-9076-4762-b31f-3ceb79989b66.png)


![separator2](https://i.imgur.com/4gX5WFr.png)



# ⦿ Branching
## Create branches and move between them
> ### `git branch`
> - return all branches in repo 
> - \* sign to the current branch
> 
> ### `git branch branch_name`
> - Create branch with branch_name
> 
> ### `git checkout branch_name`
> - Travel between branches
> 
> ### `git checkout -b branch_name`
> - Create the branch and travel to it
> 
> ### `git branch -m new_branch_name`
> - Rename the current branch

## Delete Branch
> `Note to travel to another branch to be able to delete the branch`
> 
> ### `git branch -d branch_name`
> - Safe mood
> - Git checks if the branch has changes that not merged yet to the master branch if (true) it will be not deleted else delete
> 
> ### `git branch -D branch_name`
> - Force mood
> - Delete the branch without checking

## Merge Branch in git 

> ### `git checkout main` `git merge branch_name`
> - Merge main branch with another branch
> 
> ## Send branch to githup 
> ### `git push origin branch_name`
> - Sent to gihhup and we can merge there
> 
![separator2](https://i.imgur.com/4gX5WFr.png)





# ⦿ Stash
## Usage 
> Used to stash [Hide] some commits that you do not want to commit now. Same mexanism of stack [Last In First Out LIFO]

## Add and get from stash 
> ### `git stash`
> - Hide files that added to staging area 
> 
> ### `git stash save "message"` 
> - add message to your stash 
> 
> ### `git stash list`
> - List stash array 
> 
> ![image](https://user-images.githubusercontent.com/99830416/220619724-c0be96af-b6f5-40da-aa59-87a0425145bc.png)
> 
> ### `git stash pop`
> - Return last elements added to stash and put it in the **staging area**( stash[0] ) and pop it [stash.top() then stash.pop()] 
> 
> ### `git stach apply`
> - Return the top of the stach **Without** removing it form stash and add it to the staging area 

## Indexing in stash 

> ### `get stash pop stash@{index}`
> - Get the stash element at index and remove it 

## Delete from stash 
> ### `git stash drop`
> - Drop the top of the stash 
> 
> ### `git stash drop stash@{index}`
> - Drop stash element at this index [NOTE : all data in this index in stash will be deleted]
 
## Display stash 
> ### `git stash show` 
> - Return the info of the top element at stash 
> 
> ### `git stash show stash@{index}`
> - Return the info of the top element at this index in the stash 

## Take Stash element to a branch 

## [WARNING] Burn your stash🔥💣
> ### `git stash clear`
> - **ALL DATA IN THE STASH WILL BE REMOVED**

![separator2](https://i.imgur.com/4gX5WFr.png)







# ⦿ Managing Files & Staging Area
## Open file on vs code
> ### `code filename`

## Unstage Files 
> ### `git restore --staged file_name`
> ![image](https://user-images.githubusercontent.com/99830416/220703090-c9639ba7-b2ec-499f-81bf-8d302e1dcff4.png)

## Clean
> ### `git clean -n`
> - List all files that can be deleted [files that not in staging area]
> 
> ### `git clean -f`
> - Remove all listed files in the previous step 
> 
> ![image](https://user-images.githubusercontent.com/99830416/220756391-6058ed5d-5663-4b37-837e-952340a9957d.png)

![separator2](https://i.imgur.com/4gX5WFr.png)







# ⦿ Managing Committs
- Each commit has ID you can get it from githup or git 
- HEAD point to the last commit

## Get info about commitss
> ### `git log` 
> - List recent commits with their ids and **HEAD** pointer that point to the last commit
> 
>   ![image](https://user-images.githubusercontent.com/99830416/220764532-6512e115-f4b2-4b02-94e7-69306bcce8dc.png)

## Delete Committs [Be Careful]
> - In case you want to delete the last commit [bad commit], make Head point to the next commit [good commit]
> - In case you want to delete top 2 commits make head point to the third commit from top 
> 
> ### `git reset --hard Good_commit_id`
> - Now Head is at Good commit
> ### `git push origin main --force`
> - Update the remote repo with this update
> - Bad Commit will be **REMOVED**
> 
> ![image](https://user-images.githubusercontent.com/99830416/220765625-fe7f49f7-852f-4ca2-841b-8a8a54674122.png)
> ![image](https://user-images.githubusercontent.com/99830416/220766419-cb876d4b-b86d-4a8f-b5ef-5c9800d20440.png)

![separator2](https://i.imgur.com/4gX5WFr.png)
