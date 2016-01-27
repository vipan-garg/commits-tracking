# commits-tracking
here's the summary of how we avoided merge commits:

git checkout master
git checkout -b feature/foo

# make some commits

git rebase master
git checkout master
git merge --ff-only feature/foo


# above should to the trick.
