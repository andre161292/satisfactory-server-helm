# Satisfactory Dedicated Server Helm Chart

This chart deploys a dedicated Satisfactory server in your k8s stack.

# Usage

## Pre-requirements

You need to have a LoadBalancer installed and all three ports (see [Config](#Config)) unused, in order for this chart to work.

## Install/Upgrade

1. Add helm repo:
   ```
   helm repo add andre161292-github https://andre161292.github.io/satisfactory-server-helm/
   ```
2. Install to your cluster:
   ```
   helm upgrade satisfactory andre161292-github/satisfactory -n game-servers --install --create-namespace
   ```

## Config

Have a look at [values.yaml](charts/satisfactory/values.yaml) for available options.

See https://github.com/andre161292/satisfactory-server for more information about the values used. 
