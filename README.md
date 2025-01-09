Welcome to git-commands-onboarding

To copy this repository in your machine, I assume you've installed [`Git`](https://git-scm.com/downloads), you'll also need to login to your Remote Git Provider e.g. ([GitHub](https://github.com), [GitLab](https://gitlab.com/), [Azure DevOps](https://dev.azure.com/), etc.) if you want to clone private repository in your machine, or if you want to push your local git repository in your chosen Remote Git Provider, you can do this by running this in your terminal:

```bash
    gh auth login
```

After successful login, you may access your remote Git Repository in your local machine.

| Table of contents                        |
| ---------------------------------------- |
| [Git Remotely](#git-remotely)            |
| [Git Locally](#git-locally)              |
| [Git Actual Applications](#git-actually) |

#### Git Remotely

Clone Remote repository to your machine:

```bash
    git clone <HTTPS/SSH_ORIGIN>
```

Pushing local Git to remote:

First and foremost you need to initialize a target origin to push through:

```bash
    git remote add origin <HTTPS/SSH_ORIGIN>
```

New branch _(not yet existing in Remote Git Provider)_:

```bash
    git push --set-upstream origin <BRANCH_NAME_YOU_WANT_TO_PUSH>
```

Existing branch in Remote Git Provider:

```bash
    git push origin <BRANCH_NAME_YOU_WANT_TO_PUSH>
```

Or if you are in the branch that you want to push you can omit origin and branch name:

```bash
    git push
```

#### Git Locally

No Git repository is possible without this command, behold!:

```bash
    git init
```

Add local changes like new file, new line in a file, basically everythin new in you local git repository:

```bash
    git add <NEW_FILE>
```

Don't forget the file extension! nyahahaha.

You can also add all changes with one `Git` command with the power of DOT! which targets the current directory:

```bash
    git add .
```

Using the add command in `Git` is like passengers taking a seat inside a Jeepney, which means you can also exclude file you don't want to be added in your local `Git` by the opposite of add, which is:

```bash
    git rm <SUSPECT_FILE!>
```

Or all suspect files!:

```bash
    git rm .
```

Suspect? Err... I mean unwanted files.

After adding files and you're confident in your changes, you are not yet done, you need the power of:

```bash
    git commit -m <MESSAGE_HERE>
```

You can now view your commit history in your terminal by running:

```bash
    git log --pretty="oneline"
```

You can then check your current branch with:

```bash
    git branch
```

Or to view all branch:

```bash
    git branch -a
```

If you want to push to your chosen Remote Git Provider go [here](#git-remotely).

#### Git Actually

This section provides the actual example of git commands in action:

**Adding**

```bash
    git add text.txt
```

```bash
    git add .
```

**Removing**

```bash
    git rm text.txt
```

```bash
    git rm .
```

**Cloning**
_HTTPS_:

```bash
    git clone https://github.com/nikitimi/git-commands-onboarding.git
```

_SSH_:

```bash
    git clone git@github.com:nikitimi/git-commands-onboarding.git
```

**Adding Remote Origin**:

```bash
    git remote add origin git@github.com:nikitimi/git-commands-onboarding.git
```
