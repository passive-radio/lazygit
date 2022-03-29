# lazygit

## Open global or your repository git config file and add these lines below.

1. How to edit global git config file
    ```bash
    vim ~/.gitconfig
    ```

1. How to edit local git config file
    ```bash
    vim .git/config
    ```

3. Codes to be added
    ```conf
    [alias]
        p = "!f(){ git add.; git commit -a -m \"$1\"; git push -u origin HEAD;};f" # add, commit push in one line
        change = "!f(){ git branch $1; git checkout $1;};f" # make new branch, checkout to new branch in one line
    ```
