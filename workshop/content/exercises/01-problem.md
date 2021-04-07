
1. Execute a dry-run command to create, in yaml format, the resource definition for a namespace named `frontend`.  Write the yaml output to the file `my-namespace.yaml`.

    ```examiner:execute-test
    name: core-ns-spec
    title: Manifest for namespace created
    autostart: true
    ```

```section:begin
title: Solution
```

```bash
k create ns frontend --dry-run=client -o yaml > my-namespace.yaml
```

Alternatively, use the `DR` environment variable as a shorthand:

```bash
k create ns frontend $DR > my-namespace.yaml
```

```section:end
```
