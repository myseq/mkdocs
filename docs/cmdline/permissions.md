---
icon: material/console-line
title: Permission
---

# Fix Permissions

This is to change the 777 permissions to 755 for folders and 644 for files.

For files:

```console
% find . -type f -exec chmod 644 {} \;
```

For directories:

```console
% find . -type d -exec chmod 755 {} \;
```


