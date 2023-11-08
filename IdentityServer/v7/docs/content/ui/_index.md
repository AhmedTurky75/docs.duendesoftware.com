+++
title = "User Interaction"
description = "Overview"
weight = 40
chapter = true
+++

# User Interaction and Pages

The design goal of Duende IdentityServer is to supply a full implementation of the OpenID Connect protocol while on the same time be the most flexible and extendible solution. One area that is customized in all deployments of IdentityServer is the user interface. It is typically branded to have the same look and feel as other web sites of the organization. The logic driving the pages is also closely related both to the design and the business rules. To allow full flexibility of the UI, including business rules and user flow, the UI is separated from the core IdentityServer product.

![Overview](images/host.png)

To get a quick start with the UI, we provide a [quick start UI]({{< ref "./../quickstarts/2_interactive#add-the-ui">}}) as well as a [quick start UI adapted to Asp.Net Identity]({{< ref "./../quickstarts/5_aspnetid">}}).

## Required Pages

As browser requests are made to the protocol endpoints in your IdentityServer, they will be redirected to the interactive pages for the user to see. Depending on the features required, the pages expected in your IdentityServer are:
* [Login]({{< ref "./login" >}}): allows the user to login. This could be achieved with a local credential, or could utilize an external login provider (e.g. social or enterprise federation system).
* [Logout]({{< ref "./logout" >}}): allows the user to logout (including providing single sign-out).
* [Error]({{< ref "./error" >}}): display error information to the end user, typically when there are workflow errors.
* [Consent]({{< ref "./consent" >}}): allows the user to grant resource access to clients (typically only used if the client is third-party).

[Additional custom pages]({{< ref "./custom" >}}) that you might want are then also possible (e.g. password reset, registration), and those are typically available to the user as links from one of the above pages.

