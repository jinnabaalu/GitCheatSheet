# Create Branch

## Checkout to the upstream branch

**Why we need a new branch ?**

When you are working on the feature assigned you to work on, you need to work on your own branch so that your code change will not effect the others or the parent branch.

**Where we need to create the branch ?**

Identify your parent branch from where you can create your branch. Most of the time the feature branches will be created from `develop` branch.

**What are the types of branches we generally use?**

There isn't any single standard for types of branches. Git provides us freedom to create our own branching strategy. The very Generic standard I follow here. 

##### Dev Branches
- `main` - production code, released for end user.
- `develop` - branch for development, where any developer can create their branch from here and work on their own feature.
- `featureBranch` - task based branch name, we can name it with any naming convention. Example Branch Named: jinnabalu/HomePageDesign, feature/HomePageDesign, ENG-2312/HomePageDesign
- `hotfix` - we create the hotfix branch from the `main` when the end user faces issues in the live application, and we need to fix. 
##### Ops Branches

- `staging` - branch is like `main` released to the staging environment.

## Create the branch 

- Checkout to the branch `develop`, if you are a developer and got a task to work on a new feature.

```bash
git checkout develop
```

## Pull Latest

- Get latest changes because there might be changes pushed by some other developers from your last pull. 

```bash
git pull
```

## Create a new branch

```bash
git checkout -b jinnabalu/branchName
```

`jinnabalu`: the user name of the GitHub, to recognize the user by branch name easily when working with the team

`branchName`: branchName for readability we maintain [NamingConvension](https://github.com/JinnaBalu/GitCheatSheet/blob/master/NamingConvension.md#naming-convention-for-programming) for naming the branch.

