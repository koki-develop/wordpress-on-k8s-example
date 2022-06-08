クラスターを構築

```
$ kind create cluster --config kind.yaml
```

Ingress NGINX を導入

```
$ kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/kind/deploy.yaml
```

起動

```
$ kubectl apply -k ./manifests/overlays/local/
```
