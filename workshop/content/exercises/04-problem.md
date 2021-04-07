
1. Generate a pod manifest file `mypodx.yaml` (in your current working directory). Pod name should be `mypodx` with image `redis`. Make sure you only generate the pod manifest file, you do not have to create the pod.

    ```examiner:execute-test
    name: core-redis-pod-manifest
    title: Pod yaml has correct name and image
    autostart: true
    ```

<div style="margin-top: 5em;"></div>

```section:begin
title: Solution
```

1. Generate a pod manifest file `mypodx.yaml` (in your current working directory). Pod name should be `mypodx` with image `redis`. Make sure you only generate the pod manifest file, you do not have to create the pod.

    ```bash
    k run mypodx --image=redis --dry-run=client -oyaml > mypodx.yaml
    ```

```section:end
```
