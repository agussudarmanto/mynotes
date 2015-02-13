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

