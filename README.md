Awx Deploy
=========

# Ansible Role: awx_deploy

This role deploys the **AWX Operator** and an **AWX instance** on OpenShift.

## Requirements
- OpenShift CLI (`oc`)
- Git + Make installed
- Ansible >= 2.9

## Role Variables (defaults)

```yaml
awx_version: "24.0.0"          # Must be >= 24.0.0
namespace: "awx"               # OpenShift namespace
awx_instance_name: "awx-demo"  # AWX CR name
ingress_type: "Route"          # Route | ClusterIP | LoadBalancer
