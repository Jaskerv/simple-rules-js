Run:

```
bazel build //...
```

See Error:
```
ERROR: no such package '@npm//': 
ERROR: in verify_node_modules_ignored:
pnpm install will create nested node_modules, but not all of them are ignored by Bazel.
We recommend that all node_modules folders in the source tree be ignored,
to avoid Bazel printing confusing error messages.

Either add line(s) to //:.bazelignore:

node_modules

or disable this check by setting 'verify_node_modules_ignored = None' in `npm_translate_lock(name = "npm")
```
