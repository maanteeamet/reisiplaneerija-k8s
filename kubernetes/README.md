# Right now just some things to remember and do

## Setup registry

kubectl create secret docker-registry peatusee --docker-server=registry.mnt.ee --docker-username=peatusee --docker-password=<password> --docker-email=info@opennodecloud.com

## Create POD-s

```
NAMESPACE="peatus-development"

kubectl apply -f priority-classes.yml --namespace peatuselopment
kubectl apply -f hsl-map-server.yml  --namespace $NAMESPACE
kubectl apply -f pelias-data-container.yml --namespace $NAMESPACE
kubectl apply -f pelias-api.yml --namespace $NAMESPACE
kubectl apply -f digitransit-ui-default.yml --namespace $NAMESPACE
kubectl apply -f pelias-interpolation.yml --namespace $NAMESPACE
kubectl apply -f digitransit-proxy.yml --namespace $NAMESPACE
kubectl apply -f navigator-server.yml --namespace $NAMESPACE
kubectl apply -f mosquitto-server.yml --namespace $NAMESPACE
kubectl apply -f gtfs-rt-server.yml --namespace $NAMESPACE
kubectl apply -f opentripplanner-estonia.yml --namespace $NAMESPACE
kubectl apply -f opentripplanner-data-con-estonia.yml --namespace $NAMESPACE
kubectl apply -f pelias-interpolation.yml --namespace $NAMESPACE
kubectl apply -f pelias-pip.yml --namespace $NAMESPACE
kubectl apply -f rt-estonia-vehicles-service.yml --namespace $NAMESPACE
kubectl apply -f pelias-interpolation.yml --namespace $NAMESPACE
kubectl apply -f pelias-libpostal.yml --namespace $NAMESPACE
kubectl apply -f pelias-pip.yml --namespace $NAMESPACE
kubectl apply -f pelias-placeholder.yml --namespace $NAMESPACE
```
