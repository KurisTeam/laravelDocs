## Github Git Commands list

- git config

  `This command sets the author name and email address respectively to be used with your commits`

```
git config –global user.name “[name]”
git config –global user.email “[email address]”
git config –global user.name "abcd"
git config –global user.email "abcd@gmail.com"
```

- git status

  `This command lists all the files that have to be committed`

```
git status
```

- git init

  `This command is used to start a new repository.`

```
git init [repository name]
git init
```

- git add

  `This command adds a file to the staging area`

```
git add [file]
git add .
git add *
```

- git commit

`This command records or snapshots the file permanently in the version history`

```
git commit -m “[ Type in the commit message]”
git commit -m 'initial commit'
```

- git push

`This command sends the committed changes of master branch to your remote repository`

```
git push [variable name] master
git push [variable name] [branch]
git push –all [variable name]
git push [variable name] :[branch name]

```

- git pull

`This command fetches and merges changes on the remote server to your working directory.`

```
git pull [Repository Link]
```

- git remote

`This command is used to connect your local repository to the remote server.`

```
git remote add [variable name] [Remote Server Link]
```

- git merge

`This command merges the specified branch’s history into the current branch.`

```
git merge [branch name]
```

- git checkout

`This command is used to switch from one branch to another.`

```
git checkout [branch name]
git checkout -b [branch name]
```
