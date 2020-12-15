# Example - REST API and SSO

Example of Hybrid Web with RESt API and SSO (Keycloak)

REST API and Keycloak templates are stored in [drupal](components) and they need to be created manually or via argoCD.

```shell
kubectl -n restapi-sso-dev create -f components
```

SSO is accessible under `/auth/` context and api under `/api/yellow`.