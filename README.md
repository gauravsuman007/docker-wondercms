# docker-wondercms
Docker image for WonderCMS, a flat file CMS (<https://www.wondercms.com/>).

This image sets up a development environment and relies on Debian Linux, Apache 2 and PHP7.

## How to use this image
First pull the laest release from wondercms (replace the version number as needed)
```
git clone --depth 1 https://github.com/robiso/wondercms.git -b 3.4.2 <website_folder_name>
```

This will start a Wonder CMS instance listening on port 80:


```
$ docker run -d -p 80:80 --name wondercms -v ./<website_folder_name>:/var/www/html gauravsuman007/wondercms
```
