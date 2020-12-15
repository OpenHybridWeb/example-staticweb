# Example - REST API and SSO

Example of Hybrid Web with RESt API and SSO (Keycloak)

REST API and Keycloak templates are stored in [drupal](components) and they need to be created manually or via argoCD.

```shell
kubectl -n drupal-restapi-dev create -f components
```

Drupal starts with installation and needs access to postgres with:

* host=postgresql
* db=drupal_production
* username=drupal
* password=drupal

