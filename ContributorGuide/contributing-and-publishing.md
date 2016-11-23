# Major contributions and publishing

> All repositories that contribute to docs.microsoft.com content have adopted the Microsoft Open Source Code of Conduct. For more information see the Code of Conduct FAQ or contact opencode@microsoft.com with any additional questions or comments.

If you have a large contribution with several files or new files, we recommend using the following workflow for contributing content. This is the workflow content developers at Microsoft use. 

<video width="640" height="360" controls poster="./media/contributing-and-publishing/your-individual-workflow.png">
  <source src="http://video.ch9.ms/ch9/1e1b/63477be7-a3df-4d25-b8e7-9d79df411e1b/githubcontributorworkflow_mid.mp4" type="video/mp4">
  <a href="http://video.ch9.ms/ch9/1e1b/63477be7-a3df-4d25-b8e7-9d79df411e1b/githubcontributorworkflow_mid.mp4">
    <img src="./media/contributing-and-publishing/your-individual-workflow.png" alt="Your individual workflow">
  </a>
</video>

## Creating a local working branch

Whenever you work on a set of changes, it’s a good idea to create a new branch to manage those changes through the workflow.

1. Launch the Git enabled command prompt. For example, on Windows use *Git bash*, on MacOS use *terminal*, on Linux use *bash* shell.

2. Switch context to your `<repository-name>`. This is a local directory on your computer. For example, `c:\users\user-account\repository-name\` or  `/user/user-account/repository-name`

   ```
   cd <repository-name>
   ```

3. Set the current working branch to the 'master' branch:

   ```
   git checkout master
   ```

4. To create a new branch, use the `git pull` command. Note the arguments used in the command. You are pulling the *upstream* master branch and creating a branch <working branch> in the local repository.

   ```
   git pull upstream master:<working-branch>
   ```

    Now, you have a new working branch in your local repository with the latest changes from the Microsoft repository's master branch. 

5. Next, you need to switch the *current branch* to your new branch.  Use the `git checkout` command to set the current branch.

   ```
   git checkout <working-branch>
   ```

    The *current branch* is now the newly created working branch. 

6. Next, you need to sync the new working branch to your fork in GitHub.  You use the `git push` command to sync your local repository with a GitHub repository. Note the arguments used in the command. You are pushing your &lt;working branch&gt; in the local repository to *origin*. The -u switch saves the push defaults for the branch. This allows you to call future *push* commands with no arguments on this branch. 

   ```
   git push -u origin <working-branch>
   ```

## Creating and updating articles

1. Before making changes to files in your local repository, verify your working branch. Use the `git branch` command to list the branches available in your local repository.

   ```
   git branch
   ```

    The current branch is prefaced with an asterisk.

2. Now, you are ready to make changes to your local repository's working branch. You can update articles using the text editor of your choice; if you wish to create a new article, please see [Creating a new docs.microsoft.com article](./create-new-article.md).


## Committing changes to your local working branch

Git tracks a set of changes in a *commit*. A commit is a group of related changes you've made to several files. This allows you to group snapshots of changes that can be reversed if necessary. 

1. After you create/modify/delete files in your working directory, you need to "add" them to staging, then "commit" them into the branch:

   ```
   git add -A
   git commit –m "<comment>"
   ```

   Or, to add only the specific files you modified:

   ```
   git add <file path>
   git commit –m "<comment>"
   ```

4. Since updates from other contributors happen frequently, you should keep your working branch current with any new changes. To update your local working branch with changes from upstream, use the following command:

   ```
   git pull upstream master
   ```

    This gets the latest changes from the upstream master branch and merges them into your working branch. This helps you discover merge conflicts earlier.

5. Use the `git push` command to sync your local repository with your forked GitHub repository. Because you used the -u switch on the first push, no arguments are required.

   ```
   git push
   ```

    Now, all your committed changes from your local working branch are synced with your fork in GitHub.

## Opening a pull request

> If you submit a pull request with new files or significant changes to documentation or code samples, we may also need to correspond with you in the pull request, asking you to submit an online Contribution License Agreement (CLA).

A pull request enables the collaboration model on GitHub. By opening a pull request, you are asking to pull the changes from your working branch and merge them into the main repository. When you open a pull request, your changes are validated by a series of automated checks to verify it can be merged.  A person called the pull request reviewer also looks at your changes and gives you feedback if they think there is an issue with your changes.


1. When you are ready to submit your content to the upstream master branch for staging, validation, and/or publishing, go to the GitHub page for your fork. For example, github.com<GitHub-user-name>/Azure-RMS. 

2. Create a Pull Request from your fork's working branch, to the docs.microsoft.com repository's master branch. Click the *New pull request* button.

   ![New pull request button](./media/contributing-and-publishing/new-pull-request-button.png)

3. Verify your fork/branch on the right (from) and the docs.microsoft.com repo/branch on the left (to). 
   ![Pull request](./media/contributing-and-publishing/pull-request.png)

   If you scroll down, the page shows you the differences between the branches. You can validate the pull request contains the changes you expect.

4. The pull request reviewer reviews your pull request, provides feedback, and/or merges your pull request. 

5. Optionally verify your published article or changes at the appropriate `http://docs.microsoft.com/*path to-your-article-without-the-MD-extension*` URL.


## Next steps

- Back to [contributors guide](./index.md)