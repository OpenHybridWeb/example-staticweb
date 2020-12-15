# Example - Drupal and REST API

Example of Hybrid Web with Drupal plus rest api.

Drupal and RESt API templates are stored in [components](components) and they need to be created manually or via argoCD.

```shell
kubectl -n drupal-restapi-dev create -f components
```

Drupal starts with installation and needs access to postgres with:

* host=postgresql
* db=drupal_production
* username=drupal
* password=drupal

Drupal is accessible on root context and API under `/api/yellow`.