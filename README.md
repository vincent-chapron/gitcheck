# Gitcheck

Gitcheck is a script to check all changes in your git repositories.

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

I work on Symfony projects and sometimes I need to make change in my vendor.

It can be easy to lose where I change something, so I just need to use gitcheck.

```bash
gitcheck
```

Here is an example of the result:
```bash
(1) path: ./vendor/victoire/victoire/
 M composer.json


62 git repository(ies) found:
1 has/have changes,
61 is/are unchanged.


Choose a number to go to the associated repository: <cursor>
```

If you press `1` and enter, you will change directory to the associated path, here `./vendor/victoire/victoire/`
