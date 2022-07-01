---
title: "Trying out the Oracle Kubernetes Offering"
date: 2022-07-01
layout: post
---

For the masters class on _Advanced Software Engineering_ I prepared some demo on Kubernetes to illustrate core concepts like _POD_, _ReplicaSet_, _Deployment_.
The last time I did it, I relied on a local installation on my laptop, using [minikube](https://minikube.sigs.k8s.io).
This time, I used the [Oracle Cloud](https://www.oracle.com/cloud/sign-in.html), based on their academic offering.

The default dashboard did not show much kubernetes-specific information such as running pods, deployments, services and so on. So I installed the [Kubernetes Dashboard](https://github.com/kubernetes/dashboard).
Found some hints about how to install it on the oracle cloud k8s and was ready to go to talk and demonstrate _rolling updates_, _kubectl apply_ and how a _Load Balancer Service_ exposes several pods to the outside world.
