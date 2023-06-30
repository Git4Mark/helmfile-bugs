#### helm template can not download chart from the harbor with https

#### steps

1. upload the chart "ca-server-service-0.1.0.tgz" to harbor repo

```bash
helm cm-push ca-server-service-0.1.0.tgz cnp --insecure
```

2. execute helmfile template to verify chart

```bash
helmfile template -f helmfile-app.yaml
```

