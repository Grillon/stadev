# stadev : a remote dev station
[![](https://images.microbadger.com/badges/image/grillon/stadev.svg)](https://microbadger.com/images/grillon/stadev "Get your own image badge on microbadger.com")
# Table Of Contents

 - [Introduction](#introduction)
 - [Version](#version)
 - [Usage](#usage)
     - [Pull The Image](#pull-the-image)
     - [Run The Image](#run-the-image)
 - [Configuration](#configuration)
     - [Available Configuration Parameters](#available-configuration-parameters) 
 - [References](#references)

# Introduction

container de developpement

contient :

* tous ce que contient stamain
* emacs/nano
* man/net-tools/telnet/wget
* gcc/c++/ruby/perl/sbcl/java8
* gdb

# Version

Current Version: **0.0.1**

# Usage

## Pull The Image

Pull the latest image, which is *HEAD* of the git repository.

```bash
docker pull grillon/stadev
```


## Run The Image

For example.

```bash
docker run -e "STAMAIN_PASSWD=nouveauMdpDeMonChoix" -p 22 -t -i grillon/stadev
```

# Configuration

## Available Configuration Parameters

 - **STAMAIN_UID** nom uid gid
 - **STAMAIN_PUID** nom uid gid du user principal
 - **STAMAIN_GID** nomGroupe gid
 - **STAMAIN_PGID** nomGroupe gid du groupe principal
 - **STAMAIN_PASSWD** oups...

# References

 * https://docs.docker.com/engine/articles/using_supervisord/
 * https://github.com/grillon/stamain
