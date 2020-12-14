Repo for checking ansible lint
1) Install pre-commit
https://pre-commit.com/

2) Pull this repo. Role good have error for linter, but i use skip argument for commit

3) Add this to bad role

```

- name: echo2
  command: |
    "echo this failed"


```

4) try to push. It will check all roles, not only changed files. Yamllint work fine
