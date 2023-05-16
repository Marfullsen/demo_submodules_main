# Submodules in git
Demo of git submodules, main repo.

## What is a submodule?

Git submodules allow you to include another Git repository as a subdirectory within your own repository. This is useful when you want to include external code or libraries as part of your project, while still keeping them separate and allowing independent development.

## How to use

### First use

Clone the repo **using the recursive flag**.

```
git clone --recursive https://github.com/Marfullsen/demo_submodules_main.git
cd demo_submodules_main
```

### Already cloned, but update in submodule needed

Update the **submodule**:

```
git submodule update
```

Update the **submodule** manually:

```
cd external\demo_submodules_external
git pull origin master
cd ../../
git commit -am "Updated submodule"
```

### Submodule subcommands

|Subcommand|Description|
|:---:|:---|
|add|Add a new submodule to the repository|
|init|Initialize submodules for the repository|
|update|Update the contents of all submodules|
|foreach|Run a Git command in each submodule|
|sync|Update the URL of a submodule to match the .gitmodules file|
|status|Show the status of the submodule|
|summary|Show a summary of the submodule commits|
|deinit|De-initialize submodules from the repository|

## References
- [7.11 Git Tools - Submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules)
- [Git docs - git-submodule](https://git-scm.com/docs/git-submodule)
- [Main repo.](https://github.com/Marfullsen/demo_submodules_main.git)
- [External repo.](https://github.com/Marfullsen/demo_submodules_external.git)
