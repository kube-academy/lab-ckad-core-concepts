
1. Create a Pod named ``nginx``{{copy}} in the namespace ``{{session_namespace}}-apps``{{copy}}, using the image ``bitnami/nginx``{{copy}}.

    ```examiner:execute-test
    name: core-make-pod
    title: Pod nginx exists
    autostart: true
    ```

<div style="margin-top: 5em;"></div>

```section:begin
title: Solution
```

```bash
k run nginx --image=bitnami/nginx -n {{session_namespace}}-apps
```

Hint:  Use the `-w` flag to see the pod status progress to running state:

```bash
k get pod -n {{session_namespace}}-apps -w
```

```section:end
```
