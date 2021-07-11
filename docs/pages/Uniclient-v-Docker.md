---
title: Uniclient v Docker
layout: default
excerpt: The easiest way to start the Universa `uniclient` on a Mac development machine is to engage at the Terminal with the `Docker Desktop` running in the background ...
hint: You will be creating a new `user preferences` sub-directory ...
repo: Universa-Lessons-Project
ver_date: 07-08-21
navigation_weight: 8
categories: page
---
{% include toc.md %}

## Environment

> **Hint**. {{ page.hint }}

### Help Switch

Adding the switch `--help` to your `docker run` command will reveal a list of available arguments, as follows:

From a base Terminal window  with your copy of `Docker Desktop` running in the background ...

```javascript

docker run universa/uniclient --help

```

### Network Switch

Adding the switch `--network` to your `docker run` command will generate a new `private key`, as follows:

From a base Terminal window  with your copy of `Docker Desktop` running in the background ...

```javascript

docker run universa/uniclient --network

```

Returns ...

"User private key is not set, generating a new one."

And,

"New private key has been generated."

**Note**. A preferences file was also removed in the background at:

`/root/.java/.userPrefs/prefs.xml`

Plus, a new `private key` has just been generated and stored within the `/root/.universa` subdirectory

#### Confirmation

`Universa network is active, 27 node(s) are reachable ...`

## Docker Desktop

**Note**. The Terminal program will engage directly with the `Universa Network` via the `Universa Client Tool` or `Uniclient` while the `Docker Desktop` is running in the background [[1](#DOCKERDESKTOP){:.red}].

## Sources

The above synopsis was derived from an article written by the `Universa Node Managers` for the `Universa Client Tool` or `Uniclient`, Network ver 3.14.4 [[1](#UNIVERSAUNICLIENT){:.red}].

***

1. {:#DOCKERDESKTOP}[Download Docker Desktop for Mac](https://hub.docker.com/editions/community/docker-ce-desktop-mac){:target="_blank"}

2. {:#UNIVERSAUNICLIENT}[The Universa Uniclient User Manual](https://lnd.im/UniClientUserManual){:target="_blank"}

***

{% include patreon-link.md %}
