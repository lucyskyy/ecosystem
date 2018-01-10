# The Revas Project: Contributing guide

**Welcome to the Revas Project!** :heart: Thank you for considering contributing to this ecosystem. [The Revas Project](https://github.com/revas) and [Revas Ltd.](https://github.com/revas-io) are **completely open**. If this is your first open source project, you can read the [Open Source Guide: How to Contribute](https://opensource.guide/how-to-contribute/).

## Code of Conduct

Before any contributing, read the [The Revas Project: Code of Conduct](https://github.com/revas/ecosystem/blob/master/CODE_OF_CONDUCT.md) so that you can understand what actions will and **will not be tolerated**.

## Issues

You can use the GitHub Issues to submit a **bug issue** or a **enhancement proposal**. Issues are the places where contributors can **discuss** and try to find a solution together. This lets the contributors reach an **agreement** on proposals before putting significant effort into it.

If you want to contribute you can start with an **existing issue**. You can also notify a bug or propose an enhancement, but please make sure the issue does not already exist.

:fire: Issues are not the place where people can ask questions, otherwise the created issue will be immediately closed. You can join our [community workspace](https://chat.revas.io) and ask in the #support channel.

:warning: If you want to submit a new issue you have to make sure it does not already exist and use the templates described in the [contributing directory](https://github.com/revas/ecosystem/tree/master/.github).

### Security bug

If you find a security bug, please **do not submit a public issue**. The security of the ecosystem is a priority, if you send an email to [project@revas.io](mailto:project@revas.io) we can solve the issue as soon as possible.

## Pull Requests

When contributors have reached an **agreement** about the issue, you can ask to implement the change. GitHub Pull Requests allow you to show your contribution to other maintainers **before merging**. With this tool you can comment and receive feedback on changes, modifying the code accordingly.

### Fork and Branch

First, you can fork the repository of interest from GitHub. Then you have to clone the forked repository on your local disk.

> Substitute `<username>` with your username and `<repository>` with the repository name.

```
$ git clone git@github.com:<username>/<repository>.git
$ cd <repository>
```

The next step is to add the source of the original repository, called upstream. Whenever you want to contribute, remember to sync with the original repository before starting.

> Substitute `<repository>` with the repository name. Discuss with the community about which is the best `<branch>` to source from. The `<working-branch>` name is usually defined by the context and the issue number, you can find more info about Git branching on [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/).

```
$ git remote add upstream git@github.com:revas/<repository>.git
$ git checkout <branch>
$ git pull upstream <branch> && git push origin <branch>
$ git checkout -b <working-branch>
```

Now you have a clean and ready workspace to work on! **Write down all your magic!** Remember that each repository has its own **style guide**. You can comment to the existing issue and ask questions about the implementation! :smile::heart:

- [ ] **Implement** new tests if needed.
- [ ] **Update** the documentation if you changed an interface.
- [ ] **Execute** the test suite.
- [ ] **Format** and **Lint** your code.

> Don't worry if you don't know these concepts. Learning is a path. Comment to the existing issue if you need help! :heart:

### Commit Messages

You can commit your progress on the local branch. We have a **guideline** for commit messages, if you follow it you make easier the the maintainers review. The GitHub desktop app helps you format the commit message and its description.

```
git commit -m ":emoji-code: <commit-message>"
```

1. Message subject must start with one emoji.
2. The subject must be less than or equal to 50 characters long with the first letter capitalized, without the period at the end of the line. *":blue_book: This is a documentation commit subject"*
9. Use the present tense and the imperative mood. *":blue_book: Add readme and license"* not ~~":blue_book: Added readme and license"~~
11. Use the Message body to explain what the commit changes.

| Emoji | Emoji Code | Description |
| :---: | :---: | :---: |
| :closed_book: | `:closed_book:` | When adding ecosystem specifications |
| :blue_book: | `:blue_book:` | When improving the documentation |
| :space_invader: | `:space_invader:` | When adding wireframes or design assets |
| :sparkles: | `:sparkles:` | When introducing a new feature |
| :zap: | `:zap:` | When introducing a new backward incompatible feature |
| :ambulance: | `:ambulance:` | When fixing a bug |
| :fire: | `:fire:` | When removing code or files |
| :recycle: | `:recycle:` | When refactoring code |
| :microscope: | `:microscope:` | When adding tests |
| :lipstick: | `:lipstick:` | When improving UI and cosmetic |
| :seedling: | `:seedling:` | When dealing with accessibility (i18n and a11y) |
| :rocket: | `:rocket:` | When dealing with deployments or dependencies |
| :whale:	 | `:whale:` | When dealing with Docker configuration |
| :gem: | `:gem:` | New Release |
| :bookmark: | `:bookmark:` | Version Tags |


### Submit a Pull Request

When you have finished the changes you can push your local branch `<working-branch>` to your forked repository.

```
git push -u origin <working-branch>
```

On the web page of your forked repository you have a new section that allows you to create a pull request to the original repository.

:fire: Pull request subject must have the form of a commit message subject without the starting emoji.

:warning: If you want to submit a new pull request you have to make sure it does not already exist and use the structure described in the [templates](https://github.com/revas/ecosystem/tree/master/.github).

> To review the full git flow used here you can refer to [The beginner's guide to contributing to a GitHub project](https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/). You can learn more on the Pull Request process on [GitHub Learning Path](https://services.github.com/on-demand/resources/learning-path/) and [Writing the Perfect Pull Request](https://github.com/blog/1943-how-to-write-the-perfect-pull-request).

### CLA

If you submit a new pull request you need to sign the CLA of the project. After your first pull request a bot will automatically ask you to access with your GitHub account to our CLA assistant. You have to do this process only once.

:fire: If you do not sign the CLA, your contribution cannot be accepted.

> The purpose of a CLA is to ensure that the guardian of a project’s outputs has the necessary ownership or grants of rights over all contributions to allow them to distribute under the chosen licence.

You can find more info about CLAs on [OSS Watch CLA](http://oss-watch.ac.uk/resources/cla).

### Merge a Pull Request

After the discussion, the community evaluate if mantain the commits of the pull request or squash them into one. The commit message subject must have the same form of a normal commit message subject with a reference to the pull request.

The mantainer that merge the pull request should close the related issue.

## Resources

Most of the time, repositories have references to **learning** resources, **architecture decision records (ADRs)** and **style guides**! :books:
