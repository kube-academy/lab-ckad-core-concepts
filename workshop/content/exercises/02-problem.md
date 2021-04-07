
1. Create a Pod named `nginx` in the namespace `{{session_namespace}}-apps`, using the image `bitnami/nginx`.

    ```examiner:execute-test
    name: core-make-pod
    title: Pod nginx exists
    autostart: true
    ```

<div style="margin-top: 5em;"></div>

```section:begin
title: Solution
```

1. Create a Pod named `nginx` in the namespace `{{session_namespace}}-apps`, using the image `bitnami/nginx`.

    ```bash
    k run nginx --image=bitnami/nginx -n {{session_namespace}}-apps
    ```

    Hint:  Use the `-w` flag to see the pod status progress to running state:

    ```bash
    k get pod -n {{session_namespace}}-apps -w
    ```

```section:end
```
