---
title:  "Kubernetes Overview"
header:
    overlay_image: "/images/kubernetes.png"
    teaser: "/images/kubernetes_teaser.jpg"
categories: 
  - devops
tags:
  - devops
  - infrastructure
  - education
---

# What is Kubernetes and why we should use it?

Kubernetes is Google’s solution to cloud management. Kubernetes
automates or “orchestrates” managing containers. So far in the container
game Docker seems to be the most popular choice. Yet, Docker has been
behind their orchestration solution where Kubernetes shine. There are
quite a few orchestration tools including Google’s Container Engine and
Kubernetes, Docker’s Swarm, CoreOS's Fleet, Amazon’s ECS, Microsoft’s
Azure Container Service. While, all orchestration tools have their pros
and cons, Kubernetes comes out on top in terms of compatibility with
platforms and popularity.

## Features: Why we should use it.
When asked “What feature from one of your competitor's platforms would
you like to have?’ A Docker Swarm representative said, “The feature set
is what I like from Kubernetes - that's why Pearson decided to go with
them; it’s is those rich features: you have daemon sets, you have
replication, you have now \[pet sets\] and they constantly add a lot of
features”. Kubernetes is a feature rich platform for lack of a better
term. Here are feature sets I found. Some of them I am not fully
familiar with. The features of Kubernetes go back to three main
categories. From Kuberetes home page, “Kubernetes is - Portable,
Extensible, and Self-healing”

-   Config map resource: key value pair makes configuration easier

-   Community driven: Scale of popularity and the nature of open source
    project makes it easy to get support, request new features, or even
    add new features on your own if you feel brave. Community support is
    available on.

-   Made by Google! They arguably have the most complex infrastructure
    and efficient infrastructure. Google made it and using it to manage
    their infrastructure.

-   Scalable: Can grow and shrink easily. Has features like load
    balancing, creating and destroying containers, health checking built
    into the core.

-   Portable/Compatible: Can integrate a combination of services. You
    could have one container/node/pod running in open stack and another
    one on AWS and it should work seamlessly.
    
## Cons: What is lacking?
These cons don’t necessarily mean that we shouldn’t be using Kubernetes
because of these issues. But rather, something we should be paying
attention to while using Kubernetes.

-   Security: In a question regarding security someone from kubernetes
    says “I would say that there's no surprise that there are a number
    of companies that spawned around Kube and one of the free leading
    features they sell would be the security scanning of the
    container system. It would be the UI, and the last would be the
    authentication authorization layer. I think that by default, that
    was something that was certainly lacking within Kube. It was not
    something that was at the forefront of the development model, but
    because they essentially mirrored the service account model that
    they use within Google Cloud, they know that they have the
    architecture to do that.” This gives me the impression that
    Kubernetes has a few security holes that 3rd party is
    converging for. However, this beauty of open source is that if there
    is one problem, there is a fleet community with multiple solution
    for the problem.

## Questions to consider before moving to Kubernetes
Questions to consider before moving to Kubernetes based infrastructure
for application:

-   Are they cloud-native?

-   Are they containerized?

-   Are they in a position that you can transfer them into containers?

-   How is the configuration set?

-   How is looking at your data?

-   How is your data managed? The persistency of your data.

-   How do we work with our deployment pipeline? 

-   How do we work with our bill pipeline?

-   How much overhead goes into deploying, maintaining and managing
    application infrastructure?
    

## Philosophy of Kubernetes:
-   Decouple: Divide application to the smallest atomic structure and
    put them in a separate container. Ex: If you have an nginx that
    serves a web page and a service that pulls from a git repo to sync
    the pages. You should put these two services in separate container.

-   Move away from host-centric to container-centric infrastructure by
    cutting the cord to physical and virtual machine.

-   Homogenous machine fleet: all the instance of an application that
    Kubernetes creates should look and feel exactly the same. So if one
    of the container dies, your application just sees that there are
    slightly less computational power available in the pool.
    
## Terms: 
-   Container: A area where an application runs isolated from a system.

-   Orchestration: Allows management of containers. Container is really
    good at modulating your application. But there is a limit to how
    much it can scale. Container can't think outside the kernel. A
    containerized system may be limited to a machine, maybe a network,
    may be an ecosystem (Think of AWS or OpenStack). Orchestration
    pushes this limit further by allowing your containers to run on a
    different system.

-   Node/Master: Each individual machine. Master is the controller of
    all the fleets of nodes.

-   Pod: Containers are grouped into pods. Will need to look up how you
    group things.

-   Kubelet: runs on each node.

## Articles/Docs:
-   <https://kubernetes.io/docs/concepts/>

-   <https://blog.outlyer.com/kubernetes-vs.-mesos-vs.-swarm>

## Other Resources:
-   [StackOverflow](https://stackoverflow.com/questions/tagged/kubernetes)
    Look for solution to problems here.

-   [Github](https://github.com/kubernetes/kubernetes/issues) "Tier 2
    support"

-   [Google
    Groups](https://groups.google.com/forum/#!forum/kubernetes-dev) In
    depth discussion of Kubernetes features and future roadmap.

###### Disclaimer: This page may be opinionated. While I will do my best to write most accurate information possible, YMMV. I am currently in the experimental phase with Kubernetes. This page is still work in progress. Also, pardon sentence structure, word choice, grammar, spelling...