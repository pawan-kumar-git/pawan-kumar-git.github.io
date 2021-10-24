#### There are lots of questions come into mind in beginners which are using git-hub first time.Here theses questions are answered 

##### FAQs
#####  Q.From where git gui downloads?
A. You can download git Gui from [Here](https://git-scm.com/downloads).

Click on  download tab as shown in figure on that page and Run it.
![GitGuiDownload](https://user-images.githubusercontent.com/91775317/138591418-90732dc5-13c9-4458-b4ab-bf2a95369d1a.PNG)

#####  Q.What is GitGui and GitBash. how to use them?

#####  Q.How to configue local git with your user name and email?
A. Use the following commends in git bash to configure it.
~~~
git config --list
git config —local user.name “ your name ”
git config —local user.email “ your email with @ ”
~~~

#####  Q.How to configue local git again, when your remove git and install with different name?
A.
   when you remove the git and install it from diferrent username.Then you try to use the git bash.Then following error will come
~~~
error: key does not contain a section: —local
~~~
To resolve that,paste the following code on the git-bash terminal. It will open global config file in VI text editor
~~~
git config --global --edit
~~~
press i to write in VI text editor and  change your user name and user email
Then,to save in VI press ESC and :wq and press enter.

#####  Q.How to add or remove remote orgin?
A.  if remote is already configured and you try to configure it again, then the following error will come
~~~
error: remote origin already exists.
~~~
Use the following command to remove origin
~~~
git remote remove origin
~~~
Check whether it got removed or not
~~~
git remote -v
~~~
Add a new remote origin such as
~~~
git remote add origin https://github.com/pawan-kumar-git/Latest.git
~~~
#####  Q.How to change Window Credential?
A. Open Git Bash in current Directory and run the following command
~~~
git config --system --unset credential.helper
~~~
### How to resolve following error
~~~
error: src refspec master does not match any
~~~
A.
This is caused by the repository still being empty. There are no commits in the repository
 and thus no master branch to push to the server. To resolve it,Create the first commit inside 
 of the repository and then it can be pushed. For example, the
 following commands will create an initial commit and push it to the server.
~~~
touch initial
git add initial
git commit -m "initial commit"
git push -u origin master
or
git push  origin master
~~~
/****************************Token Authentication********************************************************/
remote: Support for password authentication was removed on August 13, 2021. Please use a personal access
token instead
1. First of all Open This URL
2. And log in with your credentials.
3. Click on the Setting menu.
4. Then, From the Setting menu click on Developer Settings
5. Now, From the Developer Settings, menu click on Personal access token
6. From the Personal access token click on the Generate new Token button.
7. Now fill up required details like Note, Expiration, Select scopes. And then click on below Generate Token button.
8. After that new token has been generated. Copy that generated token and use this token to access Git with username
 and token.
10. If you are using Windows then please follow the below steps.
11. Open Control Panel => User Accounts => Manage your credentials => Windows Credentials.
12. It will show all generic credentials. Find your GitHub URL and click on that. Now click on the edit button. And then 
add the personal access token  generated from GitHub into the password field. And click on the Save button.
13. Now you can access Git
/********************************Important links for markdown*********************************/
####References
[1](https://pages.github.com/)
[2](https://harrywang.medium.com/how-to-host-static-markdown-web-pages-using-github-pages-61f80a3a5136)
[3](https://phuston.github.io/patrickandfrantonarethebestninjas/howto)
[4](https://www.markdownguide.org/basic-syntax/)
/***********How to fork new git hub pages*************************************/
Open your github account
paste the address from other github account on the same url
Do fork
Rename project

/********************************End of File************************************************************/
