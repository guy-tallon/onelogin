## Amazon Business

N.B I've left this based on *.co.uk* but tested on other domains.

## Onelogin Settings
<details>
<summary>Click to expand!</summary>

- Applications -> <span style="color:red">Add App</span>.
- SAML Custom Connector (Advanced)

### Info
- Amazon Business (Country)
- Icons 

### Configuration

First Header  | Second Header
------------- | -------------
RelayState  | 
Audience (EntityID)  | `https://www.amazon.co.uk`
Recipient  | `https://www.amazon.co.uk/bb/feature/sso/action/3p_redirect?idpId=1234`
ACS (Consumer) URL Validator*  | `^https:\/\/www\.amazon\.co\.uk\/bb\/feature\/sso\/action\/3p_redirect$`
ACS (Consumer) URL*  | `https://www.amazon.co.uk/bb/feature/sso/action/3p_redirect?idpId=1234`
Single Logout URL  | 
Login URL  | `https://www.amazon.co.uk/bb/feature/sso/action/3p_redirect?idpId=1234`
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
| email   | Email `*`       |
| fname   | First Name `*`        |
| lname   | Last Name `*`        |

`*` ☑️ Include in SAML assertion

## Rules

## SSO

## Acess

Assign it to yourself for testing

## Users

## Privileges

</details>

## Amazon Business Settings

<details>
<summary>Click to expand!</summary>

![amazon_bus_connection_data](img/amazon_bus_1.png)

</details>


## Troubleshooting - Extras

Error:

`Assertions could not be parsed from the request. Ensure the assertions are being sent and are encrypted by the IDP.`

- Make sure **Encyrpt Assertion** is unticked in the Onelogin Settings (yes, unticked)

