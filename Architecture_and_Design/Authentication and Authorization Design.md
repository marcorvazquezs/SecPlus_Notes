<!-- omit in toc -->
# Authentication and Authorization Design

<!-- omit in toc -->
## Topics

- [Identification and Authentication, Authorization, and Accounting (AAA)](#identification-and-authentication-authorization-and-accounting-aaa)
  - [Core Components of AAA](#core-components-of-aaa)
- [Multifactor Authentication](#multifactor-authentication)
- [Federation](#federation)
- [Authentication Technologies](#authentication-technologies)

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

- A type of authentication that requires more than just a password for account access.
- Multifactor authentication involves two or more of the types of authentication.
- Several common factors are used for authentication:
  - something you have
  - something you are
  - something you do
  - somewhere you are
- MFA provides additional security because account access requires more than a password
- Example: ATM Machine
  - Something you have - your debit card
  - Something you know - PIN number

## Federation

- Makes it possible to connect identity management systems by allowing identities to cross multiple jurisdictions or environments
- In a federated identity system, the user does not supply credentials directly to any application or service, only to the originating identity provider.
- This provides flexibility for organizations when acquisitions happen or when individual business units maintain independent authentication mechanisms across applications
- Federation and SSO are often used together but are two distinct and different concepts.

## Authentication Technologies

**Tokens**

- One of the best methods of "something you have" authentication involves using a token. Can be either a physical device or a one-time password

- **Time-based one-time password (TOTP)**: algorithm computes a one-time password from a shared secret key and the current time
- **HMAC-based one-time password (HOTP)**: algorithm that uses a shared secret and a moving factor or counter, unlike TOTP passwords, these can be valid for an unknown amount of time.

**Common Token and Similar Authentication Technologies**

| Method | Description |
|--------|-------------|
|Time-based one-time password|A one-time-use code from a hardware device or software app that provides a new code, every 30 or 60 seconds|
|HMAC-based one-time password|A one-time-use code from a hardware device of software app that provides a new code after each use|
|SMS generate one-time password|A one-time-use code sent via SMS|
|Token key|A token device that typically plugs in to a USB port|
|Static Codes|An issued set of one-time-use codes. Sometimes implemented on a static card, which uses a set of axes for cross-reference|
|Phone callback|A phone number that makes you press a number to provide a one-time code|

**Common Biometric Measures for Authentication**

| Method | Description | Issues |
|--------|-------------|--------|
|Fingerprint| Scans and identifies fingerprints | False rejection results are common. Patterns can easily be counterfeited so it is best to pair with at least on other measure. |
| Hand Geometry | Measures the length and width of a hand's profile | False rejection results are common. |
| Voiceprint | Measures the tone and pacing patterns of a spoken phrase or passage | Voices can be distorted and create false rejection results |
| Facial Recognition | Identifies and measures facial characteristics and patterns | False rejection results are common |
| Retina | Scans and identifies blood and tissue patterns at the back of the eye | False rejection results are common |
| Veins/Blood vessels | Identifies and measures patterns of blood vessels in the hand or face | False rejection results are common because of measurement inaccuracies |
| Signature | Records and measures the speed, shape of a signature | False rejection results |
| Gait | Records and measures patterns of weight shift and leg movement while walking | False rejection results |
