Check templates rendering
=========================
```
helm install nginx nginx -f values-override.yml --dry-run --debug
```

Install chart
=============
```
helm install nginx nginx -f values-override.yml
```

Update chart
============

- Edit file ```values-override.yml```

- Apply changes

    ```
    helm upgrade nginx nginx -f values-override.yml
    ```

Uninstall chart
===============
```
helm uninstall nginx
```
