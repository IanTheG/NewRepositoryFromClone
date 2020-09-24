# New Repository From Clone
How to create a new GitHub repository and clone an existing repository into it. You will have to have Git installed, and some knowledge of Git and the Terminal. I made this quick tutorial because I couldn't find something concise and clear on the web. 

1. On the GitHub website, create a new GitHub repository with the SAME NAME as the repository you want to clone. Don't create it with a README or other files. 

2. In the Terminal, navigate to your Git directory. If you don't have one type these commands:  
`cd Documents`  
`mkdir Git`  
`cd Git`  

3. Then type in `git clone` and paste in the link FROM THE RESPOSITORY YOU WANT TO CLONE to your new repository:  
`git clone https://...`

This creates a folder on your computer with the name of the repository you just cloned into it. 

4. Next type in `git branch`. If something other than `* master` appears, type `git branch -M master`. This will set the branch of the respository to the master.

5. Next type in `git remote -v` to see where Git is fetching and pushing files. It most likely is still set to the cloned repository's links.  

6. Go to your GitHub repository and copy the HTTPS link under the green clone button. Type in `git remote set-url master` and paste your link in:  
`git remote set-url master https://...`

7. Type in `git remote -v` and you should see that the fetch and push links are updated to your repository link:  
`origin https://your_link... (fetch)`  
`origin https://your_link... (push)`

8. Make edits to a file, then type in `git status` and you should see that `modified:   filename.extension` is red. 

9. Type `git add .`

10. Type `git commit -m"Message here"`. You can change the message you want to upload to GitHub. 

11. Type `git push origin master` and refresh your GitHub page. The cloned files and any updates should now be reflected in the master branch on your repository!
