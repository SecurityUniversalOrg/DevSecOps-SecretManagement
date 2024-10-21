# Kubernetes/Helm
___
* Using Secrets Store CSI Driver:
   * Install the Secrets Store CSI Driver and the Azure Key Vault provider.

* Sample Deployment YAML:
```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: app-deployment
spec:
  replicas: 1
  selector:
    matchLabels:
      app: my-app
  template:
    metadata:
      labels:
        app: my-app
    spec:
      volumes:
        - name: secrets-store-inline
          csi:
            driver: secrets-store.csi.k8s.io
            readOnly: true
            volumeAttributes:
              secretProviderClass: "azure-kvname"
      containers:
        - name: my-app
          image: your-docker-image
          volumeMounts:
            - name: secrets-store-inline
              mountPath: "/mnt/secrets"
```