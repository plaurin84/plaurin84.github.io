---
layout: post
title:  "How to install PNDA on AWS"
date:   2017-09-21 22:09:00 -0400
categories: blog
---
# What is PNDA?
PNDA is a Linux Foundation Collaborative Project. It brings multiple open source technologies together, in a manner of providing a scalable big data analytics Platform. For more details, have a look at the project's website [here](http://www.pnda.io).

# Overview
While this page is focused on the specifics of an AWS deployment for PNDA release 3.5, this overview showcases the available deployment host platforms. Keep in mind that different hosts have slightly different installation procedures.

PNDA can be installed on 4 types of hosts:
* Amazon AWS using [CloudFormation](https://aws.amazon.com/cloudformation/)
* OpenStack using [Heat](https://wiki.openstack.org/wiki/Heat)
* Bare metal using OpenStack tools ([Ironic](https://wiki.openstack.org/wiki/Ironic) and [Heat](https://wiki.openstack.org/wiki/Heat))
* Virtual Machine using [red-pnda](https://github.com/pndaproject/red-pnda)

The Virtual Machine installation is not suited for production use and only provides a minimal set of components for testing and development.

For AWS, OpenStack and Bare metal, PNDA can be used for production.

While PNDA runs a cluster of applications, one can choose not to deploy all of them. You can adapt the application set to your needs. PNDA does provide two pre-configured 'flavors':
* Pico
  \- Intended for development and learning purposes. It's a fully fledged PNDA software but does not run core services in high-availability mode and provides limited storage.

* Standard
  \- Intended for meaningful PoC and investigations at scale. It runs the core services in high-availability mode and provides reasonable storage and compute resource.

For production deployments and specific needs, flavors can be customised.

PNDA's installation requires 6 main steps:
1. Choose and prepare a host
2. Create mirror components
3. Build components
4. Stage components through the mirror
5. Configure the cluster creation process
6. Deploy the PNDA cluster

You might wonder... Why so many steps?

Well, as many businesses and real world deployments, having internet on a production system is not always an option. Also, online resources are not always dependable. The custom mirror can provides a secure and private way of deploying the application, if used properly.

My personal view of PNDA's installation is an analogy to the [Gentoo philosophy](https://www.gentoo.org/get-started/philosophy/). It's about using a tool as we see fit, providing maximum flexibility for someone's needs. The mirror and configuration system provides choices to the administrator that installs PNDA.

# Installation steps
> With Great Power Comes Great Responsibility  
> &nbsp;&nbsp;\- sudo

While it's always good practice to type your own commands, I will do my best to keep the procedures copy/paste friendly.

###### 1. Choose and prepare a host
TODO
###### 2. Create mirror components
TODO
###### 3. Build components
TODO
###### 4. Stage components through the mirror
TODO
###### 5. Configure the cluster creation process
TODO
###### 6. Deploy the PNDA cluster
