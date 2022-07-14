---
layout: post
title:  "Git Branch Cleanup Script"
date:   2022-07-13 14:51:00 -0500
categories: git zsh
---

If you are like me then you are bad about cleaning up your git branches.

Then you want to switch to one so you type `git branch` and are overwhelmed by dozens of similarly named branches.

So you want to clean them up - but everyone online is suggesting you do something like

```
$> git checkout main
$> git branch --merged | xargs git branch -D
```

to automatically delete all branches not merged into main

But you know you have branches not merged into main you want to keep! and automatically deleting a bunch of things feels bad!

If this accurately describes your life then I have good news for you because I have put together a little zsh script you can use to loop through your git branches and decide on a case by case basis whether they live or die

```
function git_branch_cleanup() {
    for branch in $(git for-each-ref --format='%(refname:short)' refs/heads/)
    do
        if ! [[ $branch =~ ^main$ ]]
        then
           read "?delete ${branch}? (Y/n)" choice
           if [[ $choice =~ ^[Yy]$ ]]
           then
               printf "\033[31m"
               git branch -D $branch
               printf "\033[0m"
           fi
        fi
    done
}

alias gbc="git_branch_cleanup"
```

*Notes:*

It's a "zsh" script and not a "bash" script because there are some differences in the `read` command.
In bash you specify prompt string with `read -p "prompt"`, in zsh it's `read "?prompt"`

