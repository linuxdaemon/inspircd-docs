<!-- This file contains a page fragment. Any changes will affect all pages that include it. -->

### `/ELINE <ident@host> [<duration> <reason>]`

If `<duration>` and `<reason>` are specified then exempts an ident@host mask from being affected by other (G, K, Z, etc) X-lines. The `<duration>` may be specified as a number of seconds or as a duration in the format 1y2w3d4h5m6s. If the duration is zero then the E-line will be permanent.

Otherwise, if just `<ident@host>` is specified, removes an exemption on an ident@host mask.

This command is only usable by server operators with ELINE in one of their `<class>` blocks.

#### Example Usage

E-lines sadie@example.com for one day with the reason "Testing":

```plaintext
/ELINE sadie@example.com 1d :Testing
```

E-lines sadie@example.com for one day with the reason "Testing":

```plaintext
/ELINE sadie@example.com 86400 :Testing
```

Removes an E-line on sadie@example.com:

```plaintext
/ELINE sadie@example.com
```
