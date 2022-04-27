# Safeops / OpsLine Technical Interview Challenge

This document is intented to describe briefly the solution developed.

## The solution
<p float="left" align="center">
<img src="https://upload.wikimedia.org/wikipedia/commons/9/91/Octicons-mark-github.svg" width="200" heigth="200"/>
<img src="https://upload.wikimedia.org/wikipedia/commons/3/39/Kubernetes_logo_without_workmark.svg" width="200" heigth="200"/>
<img src="https://www.vectorlogo.zone/logos/terraformio/terraformio-icon.svg" width="200" heigth="200"/>
<img src="https://upload.wikimedia.org/wikipedia/commons/f/ff/DigitalOcean_logo.svg" width="200" heigth="200"/>
</p>

For the repos and the pipelines Github and Github actions.

For the infrastructure I decided to use Digital Ocean as cloud provider and Kubernetes as orchestration tool.

For the infrastructure as Code I used terraform.

## Repos

There are four repos (not including this for docs) for each part of the solution, tests, wep, api and infra.

### Tests and Web

These repos are the apps you gave me initially with some small modifications to fix stuff and tests deploys, plus the code of the CI/CD pipelines.

### Tests

This repo contains a group of simple tests for each app, web and api. Also contains a pipeline for running the tests isolated.

### Infra

This is the main repo, containing all the IaaC and kubernetes manifests. It also includes two pipelines, one for deploying the IaaC in terrafor, and aother for deploying the K8s manifests.

## Application access

The application is located in this [link](http://174.138.109.152/) and has four main routes.

### Routes

* /dev/front
* /dev/api
* /prod/front
* /prod/api

The first two routes are the both applications in the dev environment, and the second two, are both applications in the prod environment.


