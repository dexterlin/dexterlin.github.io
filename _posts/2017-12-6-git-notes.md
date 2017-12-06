---
layout: post
title:  "git notes"
date:   2017-12-6 10:45:00 +0800
catagory: general
---

# TODO  
* [ ] onto


# Sum











# Problem sets

## Merge

- Refusing to merge unrelated histories

```shell
#git version 2.13.2.windows.1
$ git pull origin
fatal: refusing to merge unrelated histories
#Git does not allow this since v2.9
#solution
$ git pull origin --allow-unrelated-histories
```

## rebase

- Change the very first commit

```shell
#git version 2.7.4
$ git rebase -i HEAD~3
fatal: Needed a single revision
invalid upstream HEAD~3
# solution
git rebase -i --root
```
