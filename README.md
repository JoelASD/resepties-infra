# resepties-infra

example sealed-secret creation: 
```k create secret generic pga -n monitoring --dry-run=client --from-env-file=pga.txt -o yaml | kubeseal --controller-name sealed-secrets --format yaml > sealed-pga.yaml```