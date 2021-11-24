# Datadog (ACS)

## Capablities

| Access |	| Provisioning |	|
|--|--|--|--|
| SAML | ✅ | Create |	|
| OIDC | | Delete |	|
| WS-Federation |  | Update |	|
| Form Based |  |Just in Time|✅|

## Datadog Settings
<details>
<summary>Click to expand</summary>

| :zap: The example used is **<insert>** but it will work with any domain.   |
|-----------------------------------------|


- Applications -> <span style="color:red">Add App</span>.
- SAML Custom Connector (Advanced)

### Info
- Amazon Business (Country)
- Icons 

### Configuration

First Header  | Second Header
------------- | -------------
RelayState  | 
Audience (EntityID)  | ``
Recipient  | ``
ACS (Consumer) URL Validator*  | ``
ACS (Consumer) URL*  | ``
Single Logout URL  | 
Login URL  | ``
SAML not valid before  | 3
SAML not valid on or after  | 3
SAML initiater  | OneLogin
SAML nameID format  | Email
SAML issuer type  | Specific
SAML signature element  | Response
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
|   |        |
|   |         |
|   |         |

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


</details>


## Troubleshooting - Extras

<details>
<summary>Click to expand</summary>


</details>
