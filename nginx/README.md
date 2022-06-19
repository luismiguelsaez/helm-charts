
## Test rollout

- Install
  ```bash
  helm install nginx nginx -n examples -f nginx/values-local.yaml
  ```

- Upgrade
  ```bash
  helm upgrade nginx nginx -n examples -f nginx/values-local.yaml --set image.tag=1.20.1-alpine
  ```

- Check
  ```bash
  kubectl argo rollouts get rollout nginx
  ```
