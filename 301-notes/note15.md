# Class 15: Authentication

## What is OAuth?

OAuth is an open standard for access delegation, commonly used to grant websites or applications access to information on other websites without giving them the passwords. It's commonly used for online authorization in services like Google, Facebook, and Twitter.

### Example of Using OAuth

Imagine you're using a new app, "Photosyzer," that needs access to your Google Photos account. Instead of giving your Google credentials to Photosyzer, you authenticate directly with Google. Google then provides Photosyzer with a token granting limited access to your Photos account.

### How OAuth Works

OAuth works through a series of steps to authenticate a user:

1. **Requesting Permission**: The application requests authorization to access service resources from the user.
2. **User Authorization**: The user grants the requested permissions.
3. **Application Receives an Authorization Grant**: This grant is a credential representing the user’s authorization.
4. **Application Requests Access Token**: The application requests an access token from the authorization server by presenting authentication of its own identity, and the authorization grant.
5. **Access Token Issued**: If the application identity is authenticated and the authorization grant is valid, the authorization server issues an access token to the application.

### What is OpenID?

OpenID is an authentication layer on top of OAuth, often used together with OAuth. It allows users to be authenticated by coordinating with a third-party service.

## Authorization and Authentication Flows

### Difference Between Authorization and Authentication

- **Authentication** is the process of verifying who a user is, while **Authorization** is the process of verifying what they have access to.

### Authorization Code Flow

A secure, efficient flow mainly used by server-side applications where the source code is not exposed. It exchanges an Authorization Code for a token.

### Authorization Code Flow with PKCE

PKCE ("pixy") enhances the security of the Authorization Code Flow for public clients, often used in mobile and native applications.

### Implicit Flow with Form Post

A simplified flow optimized for clients implemented in a browser using a scripting language like JavaScript. It is less secure and recommended only in certain situations.

### Client Credentials Flow

Ideal for server-to-server authentication where the client is also the resource owner. Tokens are obtained using the client’s credentials (client id and client secret).

### Device Authorization Flow

Used for input-constrained devices that connect to a trusted device to authorize the user. The user manually enters the code provided by the device on another device with richer input capabilities.

### Resource Owner Password Flow

A flow where the resource owner's credentials are used directly as an authorization grant to obtain an access token. This flow is only recommended in trusted environments.

---

## Things I want to know more about

How to become a proficient UI designer using CSS and other tools. CSS is a beast.
