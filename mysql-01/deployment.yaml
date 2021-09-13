apiVersion: apps/v1
kind: Deployment
metadata:
  name: mysql-01
  namespace: reference-app
spec:
  replicas: 1
  selector:
    matchLabels:
      app: mysql-01
  template:
    metadata:
      labels:
        app: mysql-01
    spec:
      containers:
      - image: mysql:5.7.35
        name: mysql-01
        ports:
        - containerPort: 3306
      imagePullSecrets:
      - name: artifactory-access
