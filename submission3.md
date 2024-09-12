# Lab-3

## git cat-file -p <blob_hash> (git cat-file -p 134e3231731a3790db8d136782cc8006485e325e)

Give data inside submission2.md

## git cat-file -p <tree_hash> (git cat-file -p e50659b2d719c91727430ea322980384e5e486b9)

Give all information about commits and files in branch

100644 blob ede183da8ef201e5f5737eea502edc77fd8a9bdc    README.md
100644 blob 5738bc15a0416ad2624df13badfb235052777e79    index.html
100644 blob 7a94f7af59b8968be392288ea03179a24ffc9d9e    lab1.md
100644 blob 1b99cc0044f93f556a0f6a599c7edf2f33f4944a    lab2.md
100644 blob 134e3231731a3790db8d136782cc8006485e325e    submission2.md

## git cat-file -p <commit_hash> (git cat-file -p eeff540)

Give all information about repository and ssh

tree e50659b2d719c91727430ea322980384e5e486b9
parent 61404c02796ec8d3833ca4057696ceee8a18b185
author Dzyuba Sergey <iamsergeydzyuba@mail.ru> 1725559994 +0300
committer Dzyuba Sergey <iamsergeydzyuba@mail.ru> 1725559994 +0300


# Task 2

## git checkout -b git-reset-practice

Switched to a new branch 'git-reset-practice'

## Created commits with file.txt

## git reset --soft HEAD~1

## git reset --hard HEAD~1

HEAD is now at 83e9765 First commit

## git reflog

83e9765 (HEAD -> git-reset-practice) HEAD@{0}: reset: moving to HEAD~1
04fe51b HEAD@{1}: reset: moving to HEAD~1
fb5de25 HEAD@{2}: commit: Third commit
04fe51b HEAD@{3}: commit: Second commit
83e9765 (HEAD -> git-reset-practice) HEAD@{4}: commit: First commit
3a73296 (origin/lab3, lab3) HEAD@{5}: checkout: moving from lab3 to git-reset-practice
3a73296 (origin/lab3, lab3) HEAD@{6}: commit: submission3 with task1
248fb42 HEAD@{7}: commit: submission3
ec9924f (origin/lab2, lab2) HEAD@{8}: checkout: moving from lab2 to lab3
ec9924f (origin/lab2, lab2) HEAD@{9}: commit: Site
eeff540 HEAD@{10}: commit: lab2
61404c0 (origin/master, origin/HEAD, master) HEAD@{11}: checkout: moving from lab1 to lab2
bd84c6a (origin/lab1, lab1) HEAD@{12}: commit: Merge Strategies
c9c90d1 HEAD@{13}: commit: Signed commits
292ec76 HEAD@{14}: commit: submission1
61404c0 (origin/master, origin/HEAD, master) HEAD@{15}: checkout: moving from lab1 to lab1
61404c0 (origin/master, origin/HEAD, master) HEAD@{16}: checkout: moving from master to lab1
61404c0 (origin/master, origin/HEAD, master) HEAD@{17}: clone: from https://github.com/rationalf/F24-intro-labs.git

## git reset --hard 83e9765

HEAD is now at 83e9765 First commit

