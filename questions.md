#### Git introduction

- Is it possible to add a file and commit it at the same time?
    - yes, with the -a option to `git commit` ! E.g. `git commit -a -m <msg>`
    - note: new files will be ignored with `-a`

- Should `.gitignore` be part of the repository or not?
    - yes, so that everyone has the same experince / practice
    - also when you yourself are using different computers, you want `git status` to show the same output regardless

- How can one remove a file alltogether from the stage?
    - try it! do a change, stage it, and type `git status` - it tells you what to do. 
    - `git reset -p` or `git reset $file` (staging area)  
      ref. https://coderefinery.github.io/git-intro/05-undoing/ 
      ![](https://i.stack.imgur.com/qRAte.jpg)

- What about adding a directory to the stage? How are the files within treated?
    - actually, it's impossible to stage only the directory, git works only with files. What you would do is to stage a file within a directory. If you for some reason really need to add an empty directory to a repository, the convention is to add an empty `.gitkeep` file in that directory
    - but if you have a directory with many files you can do `git add dirname` and all the files within get staged

- when forgetting to include a comment with a git commit, the editor opens. I'm not sure what to do with this, write out does not seem like the best option, but I don't see anything else that makes sense.
    - ah yes, is it an editor you're not familiar with? if you're on linux or macos it could be that the vim editor opens by default. vim is tricky but you can set another editor to be the default (https://coderefinery.github.io/installation/git/#configuring-git). To exit vim, type `:q`
        - but opening an editor like this is useful if you want to write longer commit messages: start with short summary on line 1, then longer explanation on line 3 and below
    - 

- The fact that the .DS_Store shows up as untracked file on a Mac I guess is because I have opened the directory from the GUI?
    - yeah I think Finder on macos creates these .DS_Store files. I think it makes sense to ignore this file in your .gitignore

- In the event that someone has not had their coffee yet and accidentally starts their day with "git init",is past work lost and is pulling from the server the only way to recover the previous work?
    - this is safe and will not overwrite things that are already there


#### Collaborative Git

- any ideas as to why github uses "pull request" when it involves pushing rather than pulling?
    - I believe the terminology is based on the point of view of the master branch -> you are requesting the master branch to pull your changes

- How can a team lead create issues for other collaboraters?
    - You may assign an issue to someone this way: [Assigning issues and pull requests to other GitHub users](https://docs.github.com/en/github/managing-your-work-on-github/assigning-issues-and-pull-requests-to-other-github-users)

