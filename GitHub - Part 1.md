## GitHub - Part 1

- Login to GitHub account using https://github.com

## Creating Repository in GitHub with README.md file

- Create a new repository (it’s a container where all stuff goes) using the + sign as shown below: 

![image](https://user-images.githubusercontent.com/25001852/86895774-991bb480-c122-11ea-9e0a-0e6ab95c397b.png)

- Provide the necessary details like repository name. Select repository as Public and initialize the READMD. Click ‘Create’.

![image](https://user-images.githubusercontent.com/25001852/86910859-f3734000-c137-11ea-89cd-763ad102f971.png)

Now, your repository is created, and it looks as:

![image](https://user-images.githubusercontent.com/25001852/86910903-0b4ac400-c138-11ea-89f8-4a39e7d3e459.png)

To download the repository, we have option'Download Zip' in 'Code'. Also, there are two options to copy repository locally using ‘SSH’ and ‘HTTPS’ 

![image](https://user-images.githubusercontent.com/25001852/86896805-2e6b7880-c124-11ea-9c3e-fc7b43a47cc9.png)
![image](https://user-images.githubusercontent.com/25001852/86896922-5d81ea00-c124-11ea-852a-d0dc5d9d135a.png)

- Copy the SSHRepositoryLink on to your clipboard.

- Open the command prompt or terminal to use the GitHub commands:

-To change the directory simply use: 

`cd <name of the directory you want to change to>`

To go to the folder “Downloads” use: `cd Downloads`

Use the SSH repository link from out GitHub Repository and clone it to your local system as follows:

`git clone pastesshrepositorylinkhere`

![image](https://user-images.githubusercontent.com/25001852/86911345-ce330180-c138-11ea-9f97-966489c07c72.png)

Now, the folder is copied to my ‘Downloads’. Just check the ‘Downloads’ have you got the folder demo?

- To check my folder, enter the folder using cd command again as: 
`cd demo`

- Get the list of the files in the folder demo, use:
For Windows: `dir `
For Mac: `ls`

![image](https://user-images.githubusercontent.com/25001852/86911459-f9b5ec00-c138-11ea-8d45-7da44bbc20c1.png)

- To view the content of the file:
For Windows: `type README.md`
For Mac: `cat README.md`

- To open a README.md file:
For Windows: `notepad README.md`
For Mac: `open README.md`

- To create a new file:
For Windows: `notepad test.txt`
For Mac: `vi test.txt`

- Add to the repository: 
For Windows/Mac: `git add test.txt`

- Check the status of the file using:
 `git status`
  
![image](https://user-images.githubusercontent.com/25001852/86912050-ece5c800-c139-11ea-8046-99f987f9d644.png)

- Commit the changes in the repository using:
`git commit -m “write message here”`

![image](https://user-images.githubusercontent.com/25001852/86912336-6b426a00-c13a-11ea-8652-3df5246b5793.png)


- Push the file to remote repository using: 
`git push`

![image](https://user-images.githubusercontent.com/25001852/86912378-801efd80-c13a-11ea-8ab2-ffafb2abbb02.png)

Now, this make the changes in my GitHub repository

![image](https://user-images.githubusercontent.com/25001852/86912441-9fb62600-c13a-11ea-85ed-df150393a285.png)

## Create a repository now without README.md file

![image](https://user-images.githubusercontent.com/25001852/86912607-eb68cf80-c13a-11ea-8a51-2569f53ccdd7.png)

Copy the SSHRepositoryLink on to your clipboard as did before

- To come out from the demo folder first use
`cd ..`

- To make a directory in download folder: 
`mkdir demo1`
`cd demo1`

![image](https://user-images.githubusercontent.com/25001852/86913896-f886be00-c13c-11ea-8293-11d987521b2e.png)

- To create a readmd file use 
`echo "# demo1" >> README.md`

- Initialize the directory
`git init`

- Create and add a README.md file. You can use a normal text editor depending on which OS you are using. 
`git add README.md`

- Check the status of the file 
`git status`

- Commit the changes
`git commit -m "first commit"`

- Add the origin where we have to push the file. This is the SSHRepositoryLink you copied when you created the repository.
`git remote add origin git@github.com:mskill/demo1.git`
	
- Push the file 
`git push -u origin master`

![image](https://user-images.githubusercontent.com/25001852/86914009-31269780-c13d-11ea-8519-76d4103be861.png)

Now, the README.md file is created in our repository

![image](https://user-images.githubusercontent.com/25001852/86914078-51565680-c13d-11ea-9d36-752638d1725e.png)
