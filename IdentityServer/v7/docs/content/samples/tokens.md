---
title: "Requesting tokens"
description: "Samples"
weight: 30
---

### Extension grants and Token Exchange
[link to source code]({{< param samples_base >}}/TokenExchange)

This sample shows an implementation of the Token Exchange specification [RFC 8693](https://tools.ietf.org/html/rfc8693) via the Duende IdentityServer extension grant mechanism.

See [here]({{< ref "/tokens/extension_grants" >}}) for more information on extension grants.


### Personal Access Tokens (PAT)
[link to source code]({{< param samples_base >}}/PAT)

This sample shows how to provide a self-service UI to create access tokens. This is a common approach to enable integrations with APIs without having to create full-blown OAuth clients.

When combining PATs with the [reference token]({{< ref "/tokens/reference" >}}) feature, you also get automatic validation and revocation support. This is very similar to API keys, but does not require custom infrastructure. The sample also contains an API that accepts both JWT and reference tokens.
