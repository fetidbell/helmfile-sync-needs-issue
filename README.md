# helmfile-sync-needs-issue
Example of helmfile sync bug which ignores uninstalled needs

## Steps to reproduce
1. Execute `helmfile sync --file helmfile.yaml`
2. Execute `helm list --namespace default --all`, you will find that `chart-a` installed and no `chart-b` presented