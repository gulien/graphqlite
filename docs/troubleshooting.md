---
id: troubleshooting
title: Troubleshooting
sidebar_label: Troubleshooting
---

### Error: Maximum function nesting level of '100' reached

Webonix's GraphQL library tends to use a very deep stack. This error does not necessarily mean your code is going into an infinite loop.
Simply try to increase the maximum allowed nesting level in your XDebug conf:

```
xdebug.max_nesting_level=500
```
