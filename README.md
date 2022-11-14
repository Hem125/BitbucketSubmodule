# BitbucketSubmodule

 Linked repository on bitbucket with sub repositories
 
There are two ways

using submodule 

using subtree (preferred)

Using Submodule

You simply need to be in your root folder and then add the submodule folder.

                                       git submodule add <url>
                                       
Now when you clone the project you simply need to init and update the submodule

                                       git submodule init
                                       
                                       git submodule update
                                       
                                       git submodule update --remote --merge
                                       
Using Subtree

To bring a new subtree to a parent repository, you first remotely add it, then use the subtree add command, which looks like this:

                          git remote add remote-name <URL to Git repo>
                          
                          git subtree add --prefix=folder/ remote-name <URL to Git repo> subtree-branchname
                          
Pushing and pulling changes to and from the subtree

                                                 git subtree push-all
                                                 
                              git subtree pull-all
                              
Others

git submodule set-branch -branch <branch name> -- <submodule path>
 
git submodule add -branch example URLHERE
 
git submodule init
 
git submodule update --recursive --remote
 
https://superuser.com/questions/1600823/whats-the-benefit-of-specifying-a-branch-for-a-submodule
 
 git submodule update --remote
