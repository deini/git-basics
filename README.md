git-basics
==========

Super basic git tutorial focused on HR workflow. Feel free to create a pull request to fix/add anything.


New Assignment
--------------
Let's imagine we just got a new assignment. I'll be using underbar as an example. What do we do now?
- Find the repo in github. ```https://github.com/hackreactor/2014-01-underbar```
- **Fork** the repo in to **YOUR** account.
- Clone this newly forked repo on your machine. Make sure it's your repo and not HR's (look for your username on the url in my case *deini*) ```git clone https://github.com/deini/2014-01-underbar.git```
- Set up the upstream to **HR**'s repo ```git remote add upstream https://github.com/hackreactor/2014-01-underbar.git```
- Assuming you've been working on the master branch and commiting the changes you can push it to your repo like this ```git push origin master```

Clean Branch
--------------
So ... you decide it would be fantastic to start all over again just becase we love **underbar** and you decide to create a new branch. Since we've been working on our master branch, if we create a new one we will have all those changes too ... we don't want that. Super simple steps:
- Create a new branch by fetching it from **HR's** repo like this: ```git fetch upstream master:radBranch```
- We can go ahead and checkout to our newly created branch ```git checkout radBranch``` and it's all new and clean.
- Do some work, commit, and push it ```git push origin radBranch```


Pair Programming
--------------
So we've been working on our underbar repo alone, made some changes, commits and pushes. So now your master on GitHub has all these modifications. All of a sudden we get asked to work in pairs. No biggie, here's what you do assuming you want to work on a complete new shiny and clean branch.
- Find yourself a nice spot on the pair stations.
- Clone **HR's** repo ```git clone https://github.com/hackreactor/2014-01-underbar.git```
- Do some work ... don't forget to commit frequently!
- **\*harp noise*** Time to start wrapping up, we want to make sure to push this to our GitHub accounts.
- Make sure you push to **YOUR** repo in my case I want to create a new branch on my account named pair_programming ```git push <my git repo url> <branch you've been working on>:<new branch name for your repo>``` so for me it will be ```git push https://github.com/deini/2014-01-underbar.git master:pair_programming``` 
- Your partner could go ahead and repeat the last step with his/her repo.
- Done. All your work is now on your GitHub account.
- Wondering how to get new amazing branch on your computer and keep working? Just navigate to your local repo and do a ```git pull``` after that just do a checkout to that branch ```git checkout pair_programming```
