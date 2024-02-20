# eks-example

Set up your AWS creds with `aws configure`.

Make a Github Personal Access Token with `repo` set as the scope:

https://github.com/settings/tokens

Then export `GITHUB_TOKEN` as an environment variable with:

```
export GITHUB_TOKEN=ghp_████████████████████████████████████
```

## Create cluster

```
eksctl create cluster -f eksctl-config.yaml
```

## Delete cluster

```
eksctl delete cluster -f eksctl-config.yaml --disable-nodegroup-eviction
```
