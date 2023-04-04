# Authentication and Authorization Design

## Topics

## Identification and Authentication, Authorization, and Accounting (AAA)

- **Identification**
  - Happens when a user or device presents information such as a username, a process ID, a smart card, or another unique identifier and claims an identity
- **Authentication**
  - The process of validating an identity.
  - Happens when the user provides the right credentials, such as the correct password with a username
- **Authorization**
  - After authentication is completed the credentials are measured against a list of all known credentials to determine the access rights during the session
  - Based on security policy
- **Accounting**
  - Keeps track of the resources a user accesses by keeping a record of authentication and authorization actions
  - Accounting functions log session statistics and usage information, which can then be used for things like access control and resource usage.

### Core Components of AAA

- The device that wants to access the network is known as the *client*
- The *policy enforcement point (PEP)* is the authenticator. The PEP enforces the conditions of the client's access
- The *policy information point (PIP)* holds data relevant to the decision on whether to grant access to the client
- The *policy decision point (PDP)* is the crux of the AAA decision and is responsible for making the final decision about whether to grant access to the client
- The accounting and reporting system tracks the client network usage and reports the "who, what, where, when and why"
- Core AAA components are logical functions that can be combined and are not necessarily physical devices

## Multifactor Authentication

- Several common factors are used for authentication:
  - something you have
  - something you are
  - something you do
  - somewhere you are
- MFA provides additional security because account access requires more than a password

## Federation

- Makes it possible to connect identity management systems by allowing identities to cross multiple jurisdictions or environments
- In a federated identity system, the user does not supply credentials directly to any application or service, only to the originating identity provider.
- This provides flexibility for organizations when acquisitions happen or when individual business units maintain independent authentication mechanisms across applications
- Federation and SSO are often used together but are two distinct and different concepts.

## Authentication Technologies

**Tokens**

- One of the best methods of "something you have" authentication involves using a token. Can be either a physical device or a one-time password
