# Common Git Questions

## How to remove tracking branches no longer on remote?

If you want to do this safely with only high-level Git commands, you will need to run the following commands in order:

```
git fetch --prune
```

 To find all branches known to be deleted (any trace branch is now marked as [gone]):

```
git branch -v
```

 On each orphaned tracking branch:

```
git branch -d [branch_name]
```

