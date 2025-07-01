```bash
argocd app create nginx-argocd-01 \
    --repo git@github.com:neo515/argocdtest.git \
    --path simple \
    --dest-server https://kubernetes.default.svc \
    --dest-namespace test \
    --revision HEAD \
    --sync-policy automated \
    --auto-prune \
    --self-heal
```
