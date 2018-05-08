# MyNotes

## Git
### Proxy
Koneksi ke git server jika koneksi internet menggunakan proxy
`git config --global http.proxy http://proxy.server.com:8080`
ganti `proxy.server.com` dengan IP proxy server anda dan ganti `8080` dengan port proxy server anda misalnya `3128` 

untuk Linux `export http_proxy=http://<username>:<password>@<corporate proxy>:3128`

atau taruh di `.gitconfig` di folder anda dengan isi :

    [http]
    proxy = http://<username>:<password>@<proxy address>:<proxy port>
    [https]
    proxy = https://<username>:<password>@<proxy address>:<proxy port>

### Penggunaan umum git
#### Setting username dan email
```
$ git config user.name "YOUR NAME"
$ git config user.email "GITHUB_USERNAME@users.noreply.github.com"
$ git clone https://github.com/agussudarmanto/contoh.git
$ git remote -v
     origin	https://github.com/GITHUB_USERNAME/contoh.git (fetch)
     origin	https://github.com/GITHUB_USERNAME/contoh.git (push)
$ git remote add upstream https://github.com/agussudarmanto/contoh.git
$ git remote -v
    origin	https://github.com/GITHUB_USERNAME/contoh.git (fetch)
    origin	https://github.com/GITHUB_USERNAME/contoh.git (push)
    upstream	https://github.com/agussudarmanto/contoh.git (fetch)
    upstream	https://github.com/agussudarmanto/contoh.git (push)
$ git branch myNewBranch
$ git checkout myNewBranch
atau 
$ git checkout -b myNewBranch
$ git branch
$ git branch -v
$ git commit -a
$ git push <REMOTE_NAME> <BRANCH_NAME>
$ git push origin version-2
$ git rev-list --count master
```
##### Konflik pada Git Merge
```
# https://git-scm.com/docs/git-merge#_how_conflicts_are_presented
$ git merge --abort # untuk tidak melakukan penggabungan
$ git merge --continue # untuk melakukan penggabungan
$ git commit

# Tools
$ git mergetool
$ git diff
$ git log --merge -p <path>

# Merging
$ git merge fixes enhancements
$ git merge -s ours obsolete
$ git merge --no-commit maint
```
