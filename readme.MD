# This repo is just to learn git commands - master

## get code to local 

1. cd directory-name-here (navigate to the directory where you want the code to be copied. The below command will create a directory)
2. git clone git@github.com:acsekhar2000/learn-git-commands.git
3. cd learn-git-commands ( and use ls to see the code that is down loaded)

(All branches will be pulled to local and the default branch will be set to, usually master.)

## get code to local and set a specific branch to default.

1. cd directory-name-here (navigate to the directory where you want the code to be copied. The below command will create a directory)
2. git clone -b branch-name git@github.com:acsekhar2000/learn-git-commands.git
3. cd learn-git-commands ( and use ls to see the code that is down loaded)

## merge master into dev branch in local when there are no conflicts

1. git pull  ( to pull lastest code from github) 
2. git checkout dev  ( set the current branch to master -in this case merging to master)
3. git merge master

## overwite stage with code in dev - old dev code is gone

1. git checkout dev
2. git merge -s ours stage
3. git checkout stage
4. git merge dev

## complete overwite stage with code in dev - stage code is gone
A complete overwrite isn't merging the other content, it's abandoning it.

git checkout -B stage dev

## overwrite master with staging

#### Rename master to old-master, staging to master

$ (staging) git checkout master
$ (master) git branch -m old-master
$ (old-master) git checkout staging
$ (staging) git branch -m master

#### Force push staging (now master) into remote master

$ (master) git push origin master -f

#### Change branch names back to original

$ (master) git branch -m staging
$ (staging) git checkout old-master
$ (old-master) git branch -m master

#### Sync local master with remote master

$ (master) git fetch --all
$ (master) git reset --hard origin/master


## Once repo is created in  github, Use the below commands upload a code into that repository:

1. echo "# arjun-test01" >> README.md  
2. git init  
3. git add README.md  
4. git commit -m "first commit"  
5. git remote add origin git@github.com:acsekhar2000/arjun-test01.git  
6. git push -u origin master 

## Clone remote repository and all branches

git clone --mirror https://github.com/test/frontend.git frontend/.git

### Change into frontend directory
cd frontend

### Update git config
git config --unset core.bare

### Checkout master branch
git checkout master
