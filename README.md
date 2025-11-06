# Benchmark infra

This repo contains the IaC for benchmarking programming languages on a Kubernetes cluster.

The idea is to have a simple quotes DB and having an API for retrieving them.
Then, we make as much requests we want using a load testing tool (k6, gatling, artillery, cats, ...) and compare the results in Grafana.

Let's make it !

## Tools

This project uses a GitOps approach using FluxCD for managing the cluster state. As a minimal requirement, a minimal k8s cluster should be up and running. It can be provisioned in any way you want. (I might add scripts or Terraform later + min. system requirements ?)
