# Setup
1. copy `.env.example` to `.env`
2. Modify values
```
MONGODB_CONNECTION_URI=
TOKEN_KEY=shouldbeverysecure
```
3. Run command
```
kubectl create configmap deploy-config --from-env-file=.env --dry-run=client -o yaml > kubernetes/configmap.yaml
```