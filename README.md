# nginx based on alpine:3.8 with nginx-dav-ext-module

Please notice, that these image is just a base image which includes all the dependencies you need to run a nginx with webdav-ext methods. The configuration for webdav itself is not included!  

## Motivation

Getting a webdav running with nginx on a raspberry pi is easy with the offical image. But nginx-dav-ext-module is currently not supported, so I had to do it by my own. Result is, that I used the code from [arut/nginx-dav-ext-module](https://github.com/arut/nginx-dav-ext-module), changed the [original Dockerfile](https://github.com/nginxinc/docker-nginx/blob/1fe92b86a3c3a6482c54a0858d1fcb22e591279f/mainline/alpine/Dockerfile) and done the build from scratch. After a long time of compiling it finally works! 
