# OAuth2.0 monorepository system

**The OAuth 2.0 authorization framework** - is a protocol that allows a user to grant a third-party website or application access to the user's protected resources, without necessarily revealing their long-term credentials or even their identity.

_Auth_ in the name stands for _authorization_, not _authentication_.

**Authentication verifies the identity of a user or service, and authorization determines their access rights.**


# Introduction

## Roles or terminology

An OAuth 2.0 flow has the following roles:

- **Resource Owner**: Entity that can grant access to a protected resource. Typically, this is the end-user.
- **Resource Server**: Server hosting the protected resources. This is the API you want to access.
- **Client**: Application requesting access to a protected resource on behalf of the Resource Owner.
- **Authorization Server**: Server that authenticates the Resource Owner and issues access tokens after getting proper authorization. In this case, Auth0.


## Flows or grant types

Also, there are a couple of flows (**grant types**) with different implementations and purposes of use.

OAuth 2.0 defines four flows to get an access token. These flows are called grant types.
**[Deciding which one is suited for your case](https://auth0.com/docs/get-started/authentication-and-authorization-flow/which-oauth-2-0-flow-should-i-use)**depends mostly on your application type.

- **[Authorization Code Flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow)**: used by Web Apps executing on a server. This is also used by mobile apps, using the**[Proof Key for Code Exchange (PKCE) technique](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow-with-proof-key-for-code-exchange-pkce)**.
- **[Implicit Flow with Form Post](https://auth0.com/docs/get-started/authentication-and-authorization-flow/implicit-flow-with-form-post)**: used by JavaScript-centric apps (Single-Page Applications) executing on the user's browser.
- **[Client Credentials Flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/client-credentials-flow)**: used for machine-to-machine communication.
- **[Resource Owner Password Flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/resource-owner-password-flow)**: used by highly-trusted apps.

More about every flow you can watch [here](https://www.youtube.com/watch?v=3pZ3Nh8tgTE)
or read [An introduction to OAuth 2 by DigitalOcean](https://www.digitalocean.com/community/tutorials/an-introduction-to-oauth-2).

Current project's system has been implemented using [Authorization Code Flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow), the most secure of all flows.


## Authorization code flow description

Below step-by-step authorization code flow description can be found.


# Project description


### References and contact

- [OAuth 2.0 Authorization framework documentation by Auth0](https://auth0.com/docs/authenticate/protocols/oauth)
- [More about OAuth 2.0 by Auth0](https://auth0.com/docs/get-started/authentication-and-authorization-flow/which-oauth-2-0-flow-should-i-use)
- Developer contact - [bl4drnnr@protonmail.com](mailto:bl4drnnr@protonmail.com)

Project is [MIT licensed](LICENSE).
