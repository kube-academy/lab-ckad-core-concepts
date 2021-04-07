
Run the script `check-core-concepts` to verify your solutions.

```terminal:execute
command: check-core-concepts
```

## Cleanup

Before proceeding to the next section, delete the pods you created in this section:

```terminal:execute
command: k delete pod --all
```

..and the one created in the separate namespace:

```terminal:execute
command: k delete pod --all --namespace {{session_namespace}}-apps
```
