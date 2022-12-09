# consumer-app-helmchart

## Install the helm chart

``` helm install consumer-app --create-namespace --namespace consumer-app ./ -f values-override.yaml \
--set dockerConfigJson= \
--set configVars.KafkaBroker= \
--set configVars.ElasticUrl= \
--set configVars.ElasticPassword= \
--set image.repository=csye7125project/consumer-app:v1
```

## View pods

```
kubectl get pods 
```