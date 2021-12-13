# Datadog (ACS)

## Capablities

| Access |	| Provisioning |	|
|--|--|--|--|
| SAML | ✅ | Create |	|
| OIDC | | Delete |	|
| WS-Federation |  | Update |	|
| Form Based |  |Just in Time|✅|

## OneLogin Settings
<details>
<summary>Click to expand</summary>

| :eu: The example used is **EU** but it will work with the US domain.   |
|-----------------------------------------|
<br>
| :zap: Get your **ID** /url from https://app.datadoghq.eu/organization-settings/login-methods/saml   |
|-----------------------------------------|


https://app.datadoghq.eu/organization-settings/login-methods/saml

- Applications -> <span style="color:red">Add App</span>.
- SAML Custom Connector (Advanced)

### Info

Datadog (Assertion Consumer Service)

- Icons 
    - [Horizontal](img/dd_logo_h_rgb.png "Purple and white").
    - [Square](img/dd_icon_rgb.png "Purple and white").
 

### Configuration

First Header  | Second Header
------------- | -------------
RelayState  | 
Audience (EntityID)  | `https://app.datadoghq.eu/account/saml/metadata.xml`
Recipient  | `https://app.datadoghq.eu/account/saml/assertion/id/<yourid>`
ACS (Consumer) URL Validator*  | `[-a-zA-Z0-9@:%._\+~#=]{2,256}\.[a-z]{2,6}\b([-a-zA-Z0-9@:%_\+.~#?&//=]*)`
ACS (Consumer) URL*  | ``https://app.datadoghq.eu/account/saml/assertion/id/<yourid>``
Single Logout URL  | 
Login URL  | 
SAML not valid before  | 3
SAML not valid on or after  | 3
SAML initiater  | OneLogin
SAML nameID format  | Email
SAML issuer type  | Specific
SAML signature element  | Assertion
Encrypt assertion  | [ ]
SAML encryption method  | TRIPLEDES-CBC
Send NameID Format in SLO Request  | [ ]
Sign SLO Request  | [ ]
SAML sessionNotOnOrAfter  | 1440
Generate AttributeValue tag for empty values  | [ ]
Sign SLO Response  | [ ]
SAML Encryption  | 

## Parameters

| SAML Custom Connector (Advanced) Field      | Value |
| ----------- | ----------- |
| NameID (fka Email)     | Email       |
|  eduPersonPrincipalName `*` |    Email    |
|  givenName `*` |   First Name      |
|  sn `*` |    Last Name     |
|  urn:oid:1.3.6.1.4.1.5923.1.1.1.6 `*` |    Email     |
|  urn:oid:2.5.4.4 `*` |    Last Name     |
|  urn:oid:2.5.4.42 `*` |    First Name     |

`*` ☑️ Include in SAML assertion

## Rules

## SSO

## Acess

Assign it to yourself for testing

## Users

## Privileges

</details>

## Datadog Settings

<details>
<summary>Click to expand</summary>

<ol>
    <li>Log into Datadog and go to your users (bottom left)</li>
    <li>Organization Settings -> Login Methods -> SAML</li>
    <li>Upload the Metadata File downloaded from the Datadog Applicaton you created in OneLogin</li>
    <li>✅ "Identity Provider (IdP) Initated Login" and copy the URL for 
</details>


## Troubleshooting - Extras

<details>
<summary>Click to expand</summary>

![Red Exclamation Error](img/fail.png)

If you see any error similar to the above. Upload the metadata file again. Usally works on the second attempt

</details>

