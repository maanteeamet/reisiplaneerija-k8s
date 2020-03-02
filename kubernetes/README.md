# Right now just some things to remember and do

## Setup registry

kubectl create secret docker-registry peatusee --docker-server=registry.mnt.ee --docker-username=peatusee --docker-password=<password> --docker-email=info@opennodecloud.com

## Create POD-s

```
NAMESPACE="peatus-development"

kubectl apply -f priority-classes.yml --namespace peatus-development
kubectl apply -f hsl-map-server-dev.yml  --namespace $NAMESPACE
kubectl apply -f pelias-data-container-dev.yml --namespace $NAMESPACE
kubectl apply -f pelias-api-dev.yml --namespace $NAMESPACE
kubectl apply -f digitransit-ui-default.yml --namespace $NAMESPACE
kubectl apply -f pelias-interpolation-dev.yml --namespace $NAMESPACE
kubectl apply -f digitransit-proxy-dev.yml --namespace $NAMESPACE
kubectl apply -f navigator-server-dev.yml --namespace $NAMESPACE
kubectl apply -f mosquitto-server-dev.yml --namespace $NAMESPACE
kubectl apply -f gtfs-rt-server-dev.yml --namespace $NAMESPACE
kubectl apply -f opentripplanner-estonia-dev.yml --namespace $NAMESPACE
kubectl apply -f opentripplanner-data-con-estonia-dev.yml --namespace $NAMESPACE
kubectl apply -f pelias-interpolation-dev.yml --namespace $NAMESPACE
kubectl apply -f pelias-pip-dev.yml --namespace $NAMESPACE
kubectl apply -f rt-estonia-vehicles-service-dev.yml --namespace $NAMESPACE
kubectl apply -f pelias-interpolation-dev.yml --namespace $NAMESPACE
kubectl apply -f pelias-libpostal-dev.yml --namespace $NAMESPACE
kubectl apply -f pelias-pip-dev.yml --namespace $NAMESPACE
kubectl apply -f pelias-placeholder-dev.yml --namespace $NAMESPACE
```
