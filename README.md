# Git Cheat Sheet
- [Introduction](https://github.com/JinnaBalu/GitCheatSheet/tree/master#introduction)
- [Use-cases](https://github.com/JinnaBalu/GitCheatSheet/tree/master#use-cases)
- [Naming conventions for branch names or any programming language](https://github.com/JinnaBalu/GitCheatSheet/tree/master#naming-conventions--for-branch-names-or-any-programming-language)
- [Blogs](https://github.com/JinnaBalu/GitCheatSheet/tree/master#blogs)

## Introduction

There are many questions or use cases we come across in our day to day activity,
like

- How multiple contributors can push their changes together to one project
  without any overhead? The answer is with git branching.

- Who is the contributor to the repository? only developers? The Answer is One
  who is part of the project will be the contributors in one way or the other.
  One who writes the code developer, one who writes the configurations, system
  administrator, one who creates the DevOps configurations, one who writes the
  playbooks, recipes, and pipelines.

- What is code review? is it mandatory?
- How to revert changes to the working commit?
- git vs github/gitlab/bitbucket?
- How to create the repository in GitHub/GitLab/bitbucket?
- How to initialize the repository?
- How to create the repository? git clone vs git pull?
- Difference between cloning with https:// vs git:/?
- How branching works in the case of multiple contributors?
- Best practice to resolve conflicts?
- What is a pull request? Is a pull request mandatory? and when?
- Who is the reviewer? can a bot review on behalf? and how?
- BAD or GOOD? mono repo vs poly repo?

This is an endless set of questions we have in our mind when we read about the
git and practicing git. How we get rid of the question bank about the git in the
brain? My answer would be it is an endless learning about the git, in our
day-to-day activity we do and use-cases we come across will teach us how to use
git the right way?

I will try to cover them from my experience with the different blog posts which
alone explains each topic from scratch.
## USE CASES

| **Git for developer** |  **Git for Operations**|
|--|--|
|[git config](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/git-configure.md) | [git commands for devops](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/operations-git-commands.md) |
|[git init](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/git-init.md)| [common git commands](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/commonly-used-commands.md#common-commands-using-git)  |
|[generate ssh key](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/generate-ssh-key.md)| [git for project leads/manager](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/git-for-manager-lead.md#git-for-project-leadmanager) |
|[create the repository in github(remote repository)](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/create-remote-repo.md)| [switch remote url from HTTPS to SSH](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/switch-remote-url-http-ssh.md#switching-remote-urls-from-https-to-ssh)|
|[instructions to push local changes to repository](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/git-commit-file.md#committing-files)|  |
|[create new branch](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/create-branch.md#create-branch)|  |
|[branch management](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/branch-mangement.md#single-branch-for-production-and-development)|  |
|[delete commits](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/delete-commits.md#remove-the-last-commitcommits-using-reset)|  |
|[git merge](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/git-merge.md#git-merge)|  |
|[git reset](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/reset.md#git-reset)|  |


## Naming conventions  for branch names or any programming language

- **UpperCamelCase** - `CamelCase` - Ex: `JinnaBalu`

- **lowerCamelCase** - `camelCase` (`pascalCase`) - Ex: `jinnaBalu`

- **SnakeCase** 
    - `snake_case` (`lower_case_with_underscores`) - Ex: `jinna_balu`
    - `CAPITALIZED_WITH_UNDERSCORES`
              
- **kebab-case or lisp-case** - `kebeb-case`(`hyphen-case`) - Ex: `jinna-balu``

 
## Blogs
- [Git vs Github/Bitbucket/Gitlab](https://jinnabalu.medium.com/git-vs-github-bitbucket-gitlab-1e4c064789a0)
- [Decentralized but centralized git vs GitHub/Bitbucket/GitLab?](https://jinnabalu.medium.com/git-vs-github-bitbucket-gitlab-1e4c064789a0)
- [Initialize git local repository and push first commit to remote repository (github/bitbucket/gitlab)](https://jinnabalu.medium.com/is-git-a-must-have-skill-5f72ac8c5212)
- Model of Branching (master, develop, feature, hotfix)
- Is `.gitignore` mandatory?
- Host git-server using GitLab
- Monorepo vs Polyrepo in my experience
