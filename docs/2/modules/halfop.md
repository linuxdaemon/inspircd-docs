---
title: "Module Details: halfop (v2)"
---

{! 2/_support.md !}

## The "halfop" Module

!!! warning ""
    This module has been deprecated and will be removed in the next major version of InspIRCd.

    You should use [the customprefix module](/2/modules/customprefix) instead.

### Description

This module adds channel prefix mode `h` (halfop).

### Configuration

To load this module use the following `<module>` tag:

```xml
<module name="m_halfop.so">
```

This module requires no other configuration.

### Channel Modes

Name   | Character | Type      | Parameter Syntax | Description
------ | --------- | --------- | ---------------- | -----------
halfop | h (%)     | Prefix    | `<nick>`         | Grants channel halfop status to &lt;nick&gt;.

#### Example Usage

Grants channel halfop status to Sadie:

```plaintext
/MODE #channel +h Sadie
```
