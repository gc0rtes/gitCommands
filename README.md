
ssh -T git@github.com

git@github.com:gc0rtes/static-html-website.git

1)
$ git init
# Go to GitHub interface and create a new repository with the same name, and then

2)
$ git remote add origin git@github.com:gc0rtes/myRepository.git 
(Copy the SSH link GitHub provides for your new repository.)
# tells your repository where your remote is.

3)
# create a new file. ex:
$ touch index.html 

4) 
$ git add .
# stage all files inside . working directory

5)
$ git commit -m 'First commit'
# commit the stages file with a mensage

6)
$ git push -u origin master
# sends to your remote repositore in GH your files

7)
# To clone git on current EMPTY directory. OBS: # this way it not necessary USE 'git init'
$ git clone git@github.com:user/my-project.git .

#To clone to the same name of the repository leave it in blank
$ git clone git@github.com:user/my-project.git 

#To clone to a diferent name of the repository add a name at the end

$ git clone git@github.com:user/my-project.git newRepoName


8) IGNORING FILES

create a .gitignore file.
.gitignore is a text file you must create yourself. 

Filenames inside .gitignore are ignored. Ex: fake.js

Directories inside .gitignore are ignored entirely. You can mark directories by adding a / after their name. Ex: secret/
