---
layout: exercise
title: Version Control 9
---

This is a follow up question to
[Version Control 8]({{ site.github.url }}/exercises/Version-control-8).

A colleague emails one of the team members that some of the parameter values that are being used in `rich_pred.py`
are incorrect and need to be changed urgently. Unfortunately in their haste, the colleague accidentally 
sent an old email to the other team member at the same time.

The first email said "Please go to the line that
defines `sar_parameters` and change it to

```
sar_parameters = [[22.7, 0.3], [1.2, 0.163, 0.009],
                  [14.36, 21.16], [85.91, 42.57],
				  [1082.45, 1.59, 390000000]]
```
"

The second, incorrect, email said "Please go to the line that
defines `sar_parameters` and change it to

```
sar_parameters = [[22.7, 0.3], [1.2, 0.163, 0.010],
                  [14.36, 21.45], [85.91, 42.57],
				  [1082.45, 1.59, 390000000]]
```
"

Now, follow these instructions carefully:

1.  Each team member should choose a different version and modify the file. Commit the change to each
    local repository.
2.  Both should try to push the change to the GitHub repository.
3.  One team member should get an error indicating that the commit failed because
    they aren't up to date with the repository (changes have been made since
    they last update).
4.  Pull those changes down, resolve any conflicts, and if necessary commit the correct
    version of the file.
5.  Repeat the process again so that the other team member sees and resolves the conflicts.
