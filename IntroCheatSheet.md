# The Gitpocalypse begins

### Git your bearings

Where are you? What's going on? Who am I?

Git can tell you. Bring up your command line interface and type:

```git status```

Here's how to interpret the response.

Response 1:

```fatal: Not a git repository (or any of the parent directories): .git```

Don't panic. Just like your finder folder knows you're in your Documents after
you clicked on the Documents icon, your terminal has a concept of where you're
working. Try a `cd` command then try again:
```cd \Users\MyName\Where_I_Put_My_Repository```

Response 2:

```
On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	IntroCheatSheet.md

nothing added to commit but untracked files present (use "git add" to track)
```

Don't panic even if there's red on the screen. All this means is that you typed
a change in 'IntroCheatSheet.md' (or in some other file) in the branch `master`
(or whatever branch you're in) and saved that change locally. To undo the
change, use the command, then try again.
```git checkout -- IntroCheatSheet.md```

Response 3:

```
On branch Workshop
Your branch is up-to-date with 'origin/Workshop'.
nothing to commit, working tree clean
```

WOOT. This is what we expect if we've made no changes nor checked anything out.
