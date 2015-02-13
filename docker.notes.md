# Agus Sudarmanto

## Docker notes

### Instalasi

Download file : 
[Windows Installer](https://github.com/boot2docker/windows-installer/releases/latest "boot2docker")

Install instruction : [view](https://docs.docker.com/installation/windows/)

Di dalam boot2docker berisi : VirtualBox, MSYS-git, boot2docker Linux ISO, dan Boot2Docker management tool

Menjalankan docker daemon `Boot2Docker Start`

Perintah-perintah docker :

```bash
boot2docker stop
boot2docker download
boot2docker start
docker run hello-world
$ ./boot2docker
Usage: ./boot2docker [<options>] {help|init|up|ssh|save|down|poweroff|reset|restart|config|status|info|ip|delete|download|version} [<args>]
docker run --rm -i -t -p 80:80 nginx
boot2docker ip
```

### Putty 
Download file : [Putty](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html)

- Open puttygen.exe and load ("File"->"Load" menu) the private key from `%HOMEPATH%\.ssh\id_boot2docker`
- then click: "Save Private Key".
- Then use the saved file to login with PuTTY using `docker@127.0.0.1:2022`

### Referensi
- [http://blog.thoward37.me/articles/where-are-docker-images-stored/](http://blog.thoward37.me/articles/where-are-docker-images-stored/)
- [http://forum.phalconphp.com/discussion/3710/phalcon-with-docker-boot2docker-vagrant-and-puppet](http://forum.phalconphp.com/discussion/3710/phalcon-with-docker-boot2docker-vagrant-and-puppet)
- [http://fahmpress.blogspot.com/2014/10/docker-developer-tool-berbasis-container.html](http://fahmpress.blogspot.com/2014/10/docker-developer-tool-berbasis-container.html)
- [http://andi.dirgantara.co/blog/docker-hadoop-hbase/](http://andi.dirgantara.co/blog/docker-hadoop-hbase/)