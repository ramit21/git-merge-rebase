# git-merge-rebase
merge vs rebase



## Project setup
Master was created with 2 files : file1.txt and file2.txt. A branch named 'dev-branchwas then created. Changes were checked into both master and the branch. Idea of this project is to perform merge as well as rebase from the branch onto the master, and see commit logs on how both differentiate from one another.

## Merge

Step 1) Checkout the master:
```
>git clone https://github.com/ramit21/git-merge-rebase.git
```

Step 2) Fetch the branches of the master
``` 
>git fetch
```

Step 3) Merge the dev-branch into master:
```
git merge origin/dev-branch
```

Step 4) Check the commit log:
```
git log
```

You will see the output like this:

the commit history of master and the branch will be merged as per their timestamp. And you will also see a 'merge commit' checkin as the last checking.


## Rebase

Repeat above steps in a fresh checkout-out master branch, replacing the step 3 with rebase command:

Step 1) Checkout the master:
```
>git clone https://github.com/ramit21/git-merge-rebase.git
```

Step 2) Fetch the branches of the master
``` 
>git fetch
```

Step 3) **Rebase** the dev-branch into master:
```
git rebase origin/dev-branch
```

Step 4) Check the commit log:
```
git log
```

You will see the output like this:

The commit history of master, followed by the commit history of the branch.

## References

https://medium.com/datadriveninvestor/git-rebase-vs-merge-cc5199edd77c

https://medium.com/@filissen/git-interactive-rebase-e265bb55952a

