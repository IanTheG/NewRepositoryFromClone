# New Repository From Clone
How to create a new GitHub repository and clone an existing repository into it. You will have to have Git installed, and some knowledge of Git and the Terminal. I made this quick tutorial because I couldn't find something concise and clear on the web. 

1. On the GitHub website, create a new GitHub repository with the SAME NAME as the repository you want to clone. Don't create it with a README or other files. 

2. In the Terminal, navigate to your Git directory. If you don't have one type these commands:  
`cd Documents`  
`mkdir Git`  
`cd Git`  

3. Then type in `git clone` and paste in the link FROM THE RESPOSITORY YOU WANT TO CLONE to your new repository:  
`git clone https://...`

4. Next type in `git branch`. If something other than `* master` appears, type `git branch -M master`. This will set the branch of the respository to the master.

5. Next type in `git remote -v` to see where Git is pushing and pulling files. It most likely is still set to the cloned repository's links.  

6. Go to your GitHub repository and copy the HTTPS link under the green clone button. Type in `git remote set-url master` and paste your link in:
`git remote set-url master https://...`

6. 
