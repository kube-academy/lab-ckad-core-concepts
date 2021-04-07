
1. Create a pod named `hello` with image `bitnami/kubectl` and command `echo "Hello World"`. Make sure the pod does not restart automatically.

    ```examiner:execute-test
    name: core-hello-world-pod
    title: Pod emits greeting
    autostart: true
    ```

<h2 style="margin-top: 10em;">Solution</h2>

1. Create a pod named `hello` with image `bitnami/kubectl` and command `echo "Hello World"`. Make sure the pod does not restart automatically.

    ```bash
    k run hello --image=bitnami/kubectl --restart=Never --command -- echo "Hello World"
    ```
