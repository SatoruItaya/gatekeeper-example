# gatekeeper-example

## Install Gatekeeper

```
$ helm repo add gatekeeper https://open-policy-agent.github.io/gatekeeper/charts
$ helm install gatekeeper/gatekeeper --generate-name
```

## Uninstall Gatekeeper

```
$ helm delete <release name>
$ kubectl delete crd \
    configs.config.gatekeeper.sh \
    constraintpodstatuses.status.gatekeeper.sh \
    constrainttemplatepodstatuses.status.gatekeeper.sh \
    constrainttemplates.templates.gatekeeper.sh
```

## Reference

- [open-policy-agent/gatekeeper](https://github.com/open-policy-agent/gatekeeper#how-to-use-gatekeeper)
