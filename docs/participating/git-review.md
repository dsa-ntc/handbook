# Git, GitHub, and Version Control

Whether it is code or documentation, git and GitHub are extremely helpful tools for effective collaboration in the NTC. However, git is not known for being friendly to non-technical and technical users alike, so this guide is presented as a soft introduction and a summary of best practices and learned experiences from our work in the NTC and elsewhere up to this point.

## Terminology

### Version Control

The concept of *version control* is at the heart of what makes git so powerful, but is not exclusive to git. Version control is a system that tracks changes to a file or set of files over time so that you can recall specific versions later. This is especially useful when working on a project with multiple collaborators, but it is also useful for solo projects. Version control allows you to:

- revert certain files back to a previous state
- revert the entire project back to a previous state
- inspect code history to find the source of a bug
- merge different versions of the code in a safe and traceable way
- discern what specific changes were made in the code between one version and the next
- and much more

### Git

Git is far and a way the most popular version control system in use today, with Mercurial a distant second. It is a specific implementation of version control that consists of branches, commits, and a specific set of commands to interact with the repository. Git is a command line tool, but there are many GUIs that make it easier to use.

### GitHub

GitHub is a website that hosts git repositories. It is the most popular git hosting service, but there are others such as GitLab and BitBucket. GitHub provides a web interface for interacting with git repositories, but it also provides a number of other features that make it a powerful tool for collaboration. For example, GitHub provides a way to track issues, assign tasks, and review code changes. It also provides a way to host documentation and websites and perform automated actions on code.

## Git workflows

Git is a very powerful but fairly unopinionated tool. Developers are given the freedom to use git in a way that makes sense for their project. However, this can lead to confusion and frustration when working on a project with multiple collaborators. Thus, it is helpful to establish a *workflow* that everyone agrees to follow. There are many different workflows, but the one we likely most closely emulate in the NTC happens to be called *GitHub Flow*.

### GitHub Flow

The following steps are not exclusive to *GitHub flow*, but are meant as a brief start-to-finish guide of the process. For a more detailed and specific description, see [GitHub's guide](https://guides.github.com/introduction/flow/).

1. Make sure you're on the `main` branch by using `git switch main`.
2. Run `git fetch` followed by `git status` before each working session to make sure you're working from the latest version of the docs. If you're behind, run `git pull`.
3. Create a new branch. Historically, we tend to prefix our branch names with our names or usernames and a slash. For example, if I were working on some documentation that outlines our committee's love for trains:
*[branch]: A copy of the code from the current branch that can be edited without affecting the original code. Switching branches allows you to jump back and forth between multiple versions of the same file(s).
```
git branch thomasTank/choochoo
```
4. Switch to the branch you just created:
```
git switch thomasTank/choochoo
```
5. Make your changes in a series of commits. The smaller the commits, the better, but don't commit unfinished or broken code. 
6. When you believe your code is ready for review, make one final commit and *push* your changes to GitHub:
```
git push -u origin thomasTank/choochoo 
```
!!! question "What's with the `-u origin`?"

    `origin` is the name of the online version of the repository (more generally, a *remote*). Your local version of the repository can have several `remotes` with different names. For example, if you wanted to host a copy of the docs on your personal GitHub page, you could add it as an additional remote named `personal` -u is a shortcut for `--set-upstream`. This tells git to set the remote branch you're pushing to as the *tracking branch* so that in the future you can just run `git push` or `git pull` without specifying the remote name and the branch name. (However, while you're learning git, it's helpful to use the explicit arguments instead of the defaults for practice.) If you're wondering why you didn't have to set the tracking branch on `main`, it is because `origin/main` was defined as the tracking branch when you cloned the repository. 

7. After you push, there should be a message in your terminal to initiate a pull request. Click this link or navigate to the branch on GitHub manually and click the "Compare & pull request" button. Write your pull request description in such a way that it will be easy for the reviewer to understand what you've done and why. If you need someone in particular to review your pull request, you may assign them as a reviewer.
8. It is generally a good idea to review & merge a pull request as soon as possible to reduce the number of different versions of the code we have in existence. Thus, it's a good idea to publicize your contribution in the NTC Slack and request feedback directly.
9. The Handbook Content Governance team will review your contribution. They may ask questions or make suggestions. Engage thoughtfully with the feedback process and make any necessary changes, committing to your branch and re-pushing the code. Once your contribution passes approval it will be merged by the HCG team into the main branch.

!!! question "Still confused about git and GitHub Flow?"

    Check out this short video from freeCodeCamp.org:
    <iframe width="560" height="315" src="https://www.youtube.com/embed/2GO1a1vgNrc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

!!! tip "Comradely code review"

    When reviewing a pull request, first acknowledge the volunteer effort and recognize our shared goals. Frame feedback and criticism in a way that is constructive and curious instead of dismissive or uninformed. If you have major concerns, consider setting up a conversation to get on the same page. Understand that the goal of each change is iteration, not perfection.

    When receiving feedback on a pull request, it is equally important to take feedback in stride. If you're not sure how to do this, ask for help from a more experienced contributor!

    Generally, the smaller and the more frequent the changes, the easier they are to review and the less likely there will be major issues. New contributors should attempt to make small, frequent changes and to ask for help when they need it. Core contributors should stay on top of reviewing pull requests and providing feedback in a timely manner, making sure that bottlenecks and barriers to contribution are minimized.

    Finally, the easiest, fastest, and most effective way to review code is to work on the code together, in real time. This is called *pair programming* and it is a great way to learn from each other and to build trust and camaraderie. If you're interested in pair programming, reach out in the NTC Slack!