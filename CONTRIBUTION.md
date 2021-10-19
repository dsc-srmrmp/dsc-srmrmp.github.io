---
permalink: contribution
---
## How to contribute

1. Fork the project, using the gray `Fork` button in the top right of this page
2. Make any changes in your forked repo
3. On this repo, click `Pull Requests` (which is the third option at the top of this page after the options `Code` and `Issues`) and raise a Pull Request by clicking the green `New Pull Request` button and selecting your fork from the right drop down field.

Questions can be asked by raising an `Issue`.

## How to clone repo and make changes locally after forking

- Click on the green `Code` button, then either the `HTTPS` or `SSH` option and click the icon to copy the URL. This will give you a copy of the project, so you can play around with it locally on your computer.

- Using Git on your local machine and paste in the URL. Do this to download the forked copy of this repo to your computer.

```
  git clone https://github.com/yourGithubUsername/dsc-srmrmp.github.io.git
```

- Switch to the cloned folder. This can be done with Gitbash or the integrated terminal in the VSCode editor.

```
  cd dsc-srmrmp.github.io
```

- Make a new branch. Your username would make a good branch because it's unique.

```
  git checkout -b <name-of-new-branch>
```

- Make your changes and add it to stage.

```
  git add .
```

- Commit the changes.

```
  git commit -m "Add <your-github-username>"
```

- Check the status of your repository.

```
  git status
```

- The response should be like this:

```
On branch <name-of-your-branch>
nothing to commit, working tree clean
```

- Pushing your repository to GitHub.

```
  git push origin <name-of-your-branch>
```

or

```
  git branch -M main
  git push -u origin main
```

In case you get an error message like the one below, its likely you forgot to fork the repo before cloning it. To fix this, its best to start over with the How to Contribute section above, and fork the project repo first.

```
ERROR: Permission to dsc-srmrmp/dsc-srmrmp.github.io denied to <your-github-username>.
fatal: Could not read from remote repository.
Please make sure you have the correct access rights and the repository exists.
```

- On the GitHub website, navigate to your forked repo - on the top of the files section you'll notice a new section containing a `Compare & Pull Request` button!

- Click on that button and this will load a new page, comparing the local branch in your forked repo, against the main branch in the dsc-srmrmp.github.io repo. Accept the default values in the drop down boxes and click the green `Create Pull Request` button. After creating the PR (Pull Request) our GitHub Actions workflow will add a welcome message to your PR.
  Note: A pull request allows your changes to be merged with the original project repo.

- Wait for your changes to be merged.

Hurray! You successfully made a contribution! 🎉

---

## What if I have a Conflict?

A GitHub conflict is when people make changes to the same area or line in a file. This must be fixed before it is merged in order to prevent collision in the main branch.

- To read more about this, go to [GitHub Docs - About Merge Conflicts](https://docs.github.com/en/github/collaborating-with-pull-requests/addressing-merge-conflicts/about-merge-conflicts)
- To find out about how to fix a Git Conflict, go to [Github Docs - Resolve Merge Conflict](https://docs.github.com/en/github/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-on-github)
- You can also ask for help in our [Discord server](https://discord.gg/RSrmEKfzaG) or submit an issue [HERE](https://github.com/dsc-srmrmp/dsc-srmrmp.github.io/issues/).
