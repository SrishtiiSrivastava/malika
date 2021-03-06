## GITHUB – PART 2

## Creating a file in Remote repository

Click 'Add file' to add a file

![image](https://user-images.githubusercontent.com/25001852/86914757-726b7700-c13e-11ea-8411-dbe00b06171c.png)

Provide the file name and add a description to that file. To commit the changes in the repository, click ‘Commit New File’

![image](https://user-images.githubusercontent.com/25001852/86914831-9464f980-c13e-11ea-869e-71569f13011f.png)

![image](https://user-images.githubusercontent.com/25001852/86914872-a6df3300-c13e-11ea-8c0f-b71f95601af2.png)

Adding a file remotely will not be there in the local directory. Check the files using `dir`

![image](https://user-images.githubusercontent.com/25001852/86915095-04737f80-c13f-11ea-944a-2c7cf9f06e8e.png)

As per the screenshot above, there is 1 file in the repository.

To pull the file that is added in remote repository to local repository, we use PULL command
`git pull`

![image](https://user-images.githubusercontent.com/25001852/86915220-3b499580-c13f-11ea-9ca1-1a520fbd61cc.png)

After pull, if I check the local repository using dir, there are 2 files as shown:

![image](https://user-images.githubusercontent.com/25001852/86915357-7cda4080-c13f-11ea-8550-19deeacc42a9.png)

To add a branch in master branch
`git branch branchname`

Switch the branch 
`git checkout branchname`

Adding a file in branch
`echo "#content">> filename.txt`

Then add the file and push the file. To create the branch remotely we have to use 
`git push --set-upstream origin branchname`

![image](https://user-images.githubusercontent.com/25001852/86916988-07bc3a80-c142-11ea-88c3-e395f9cfc9b3.png)

Switch the branch again to the master using
`git checkout master`

Merge command to merge the branches
`git merge mybranch`

As the merge command is used the new create branch will be merged to the master branch and the file will be inserted to it. Previously, we have 2 file in the master, now there are 3 files. Make sure to push the files using `git push`
![image](https://user-images.githubusercontent.com/25001852/86917132-3e925080-c142-11ea-859b-1652369ddd8b.png)

Now, the file which is in the branch, is now in the master branch 
![image](https://user-images.githubusercontent.com/25001852/86917264-68e40e00-c142-11ea-8f75-934002d6e1ab.png)


