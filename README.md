# Introduction

This hook can force programmers to keep consistent programming style specified by .clang-format

The pre-commit comes from **References [1]** and git-clang-format is
the same as **References [2]**

# Installation

You need to put .clang-format in the root directory of your git repository

You can download the .clang-format sample file

```bash=
$ wget https://raw.githubusercontent.com/Jim00000/clone-format-hook/master/.clang-format
```

And then install the pre-commit and git-clang-format into the .git/hooks/ directory

```
$ wget https://raw.githubusercontent.com/Jim00000/clone-format-hook/master/hooks/git-clang-format -O .git/hooks/git-clang-format
$ wget https://raw.githubusercontent.com/Jim00000/clone-format-hook/master/hooks/pre-commit -O .git/hooks/pre-commit
```

In the last, change their permissions to be executable

```bash=
$ chmod u+x .git/hooks/pre-commit
$ chmod u+x .git/hooks/git-clang-format
```


# References

- [[1] pre-commit](https://gist.github.com/alexeagle/c8ed91b14a407342d9a8e112b5ac7dab)
- [[2] git-clang-format](https://raw.githubusercontent.com/llvm-mirror/clang/master/tools/clang-format/git-clang-format)
