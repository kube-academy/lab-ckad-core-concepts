
1. Create a pod named `hello` with image `bitnami/kubectl` and command `echo "Hello World"`. Make sure the pod does not restart automatically.

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
