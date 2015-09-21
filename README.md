# Gitcheck

Gitcheck is a script to check all change in your git repositories.

## install

Clone the repository and move the script to your home.
```bash
git clone git@github.com:vincent-chapron/gitcheck.git gitcheck
cd gitcheck
mv gitcheck ~/.gitcheck
```

Update you .*shrc and load the file
```bash
# IF YOU HAVE BASH
vim ~/.bashrc
# IF YOU HAVE ZSH
vim ~/.zshrc
# ETC
```

Add the following line to your .*shrc file
```bash
source ~/.gitcheck
```
Close and re-open your terminal

## Use

I work on symfony projects and sometimes I need to make change in my vendor.

It can be easily to lost where I change something, so i just need to use gitcheck.

```bash
gitcheck
```

Here an example of the result:
```bash
(1) path: ./vendor/victoire/victoire/
 M composer.json


62 git repository(ies) found:
1 has/have changes,
61 is/are unchanged.


Choose a number to go go to the repotory associated: <cursor>
```

If you press `1` and enter, you will change directory to the path associated, here `./vendor/victoire/victoire/`
