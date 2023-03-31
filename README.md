# How to Use Git Stash
Git stash is a powerful tool that allows you to temporarily save changes in your working directory without committing them. This is useful when you need to switch to a different branch, work on a different task, or temporarily put aside unfinished changes. In this guide, we'll go over the basic usage of git stash.

## Stashing Your Changes
To stash your changes, simply run the following command:

```bash
git stash save "your stash message"
```

This command will save your changes in a stash with a message describing what you saved. If you omit the message, git will prompt you for one.

## Listing Your Stashes
To list your stashes, use the following command:

```bash
git stash list
```

This will show you a list of all your stashes, including their stash ID, description, and the branch they were made on.

## Applying Your Stash
To apply your stash, use the following command:

```bash
git stash apply [stash_id]
```

This will apply the most recent stash by default. If you want to apply a specific stash, specify the stash ID. If you don't specify a stash ID, git will use the most recent one, or ID 0.

## Deleting Your Stash
To delete a stash, use the following command:

```bash
git stash drop [stash_id]
```

This will delete the most recent stash by default. If you want to delete a specific stash, specify the stash ID. If you don't specify a stash ID, git will use the most recent one.

## Applying and Deleting Your Stash
To apply and delete your stash at the same time, use the following command:

```bash
git stash pop [stash_id]
```

This will apply the most recent stash by default and then delete it. If you want to apply and delete a specific stash, specify the stash ID. If you don't specify a stash ID, git will use the most recent one.

## Conclusion
Git stash is a useful tool for temporarily saving changes in your working directory. It allows you to switch to a different branch or task without committing incomplete changes. Remember to use `git stash list` to see a list of your stashes and `git stash apply` or `git stash pop` to apply them.
