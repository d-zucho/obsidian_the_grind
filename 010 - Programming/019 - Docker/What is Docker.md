---


title:  What is Docker
type: codingNote
alias:
topic: Docker Basics 
language: docker
tags: article

---
[Article Source]([A Beginner's Guide To Docker For Web Developers! - Usersnap](https://usersnap.com/blog/docker-for-web-developers/))


- [[#Intro|Intro]]
- [[#Containers vs VMs|Containers vs VMs]]
- [[#Docker for Web Development|Docker for Web Development]]
- [[#App Isolation for Safe Sandboxing|App Isolation for Safe Sandboxing]]
- [[#Security Benefits of Containers|Security Benefits of Containers]]
	- [[#Security Benefits of Containers#Summary|Summary]]



# Docker 

## Intro


- Tool that runs *containers* to speed up deployment of apps. 
- Creates portable, self-sufficient container from any application
	- How does it do this #review-later 
	- The same container that I build on my computer can be tested and run on VMs, in the cloud, and on other computers.

```ad-abstract
You can run a single service per container, e.g. one container for your MySQL, one container for your Apache, and one container for your WordPress installation.

Otherwise, you can put a whole application stack in one container as well. There’s no right or wrong about this.
```



## Containers vs VMs

Comparing Docker containers to VMs is a valid thing, although containers do not replace VMs. Virtual machines basically have a full operating system with its own memory management, device drivers, etc. In contrast, Docker containers share the host’s OS and are therefore much easier to manage.

![docker containers vs VMs in web development](https://ds6br8f5qp1u2.cloudfront.net/blog/wp-content/uploads/2015/06/docker-container-vs-vms-web-dev.png?x82505)


## Docker for Web Development

Instead of developing on our local engine, minimizing differences between the local environment and production can help avoid last minute changes because of configuration differences. 
- This boosts productivity and can save last minute errors and hassles


## App Isolation for Safe Sandboxing

In Docker, you run one application or process per container #docker/basics

Because of containers isolated environments, each container is assigned its own runtime evironment and receive their own network stack and process space. 

```ad-example
If you want to install different versions of pythorn, or any library, you can do this in a container and compare them with each other.
```


## Security Benefits of Containers

By running various containers, each container only has access to ports and files explicitly exposed by the other container.

Also, containers offer higher level of control on what data and software are installed. 
- *Because of this, some harmful script in one container, won't affect and other container*




### Summary

