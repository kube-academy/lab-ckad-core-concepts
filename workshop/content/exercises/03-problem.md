
1. Create a pod named ``hello``{{copy}} with image ``bitnami/kubectl``{{copy}} and command ``echo "Hello World"``{{copy}}. Make sure the pod does not restart automatically.

    ```examiner:execute-test
    name: core-hello-world-pod
    title: Pod emits greeting
    autostart: true
    ```

<div style="margin-top: 5em;"></div>

```section:begin
title: Solution
```

```bash
k run hello --image=bitnami/kubectl --restart=Never --command -- echo "Hello World"
```

```section:end
```
