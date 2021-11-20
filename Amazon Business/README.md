## Amazon Business

N.B I've left this as *.co.uk* so replace whatever domain you need.

- Add App
- SAML Custom Connector (Advanced)

### Info
- Amazon Business (Country)

### Configuration

* RelayState
    -
* Audience (EntityID)
    * https://www.amazon.co.uk

* Recipient
    * https://www.amazon.co.uk/bb/feature/sso/action/3p_redirect?idpId=<theid in the Amazon SSO Settings>

* ACS (Consumer) URL Validator*
    * ^https:\/\/www\.amazon\.co\.uk\/bb\/feature\/sso\/action\/3p_redirect$

* ACS (Consumer) URL*
    * https://www.amazon.co.uk/bb/feature/sso/action/3p_redirect?idpId=<theid in the Amazon SSO Settings>

* Single Logout URL
    * -

* Login URL
    * https://www.amazon.co.uk/bb/feature/sso/action/3p_redirect?idpId=<theid in the Amazon SSO Settings>

* SAML not valid before
    * 3

* SAML not valid after
    * 3

* SAML initiater
    * OneLogin

* SAML nameID format
    * Unspecified

* SAML signature element
    * Assertion

* SAML nameID format
    * Unsepcified

* SAML issuer type
    * Specific

* SAML signature element
    * Assertion

* Encryption assertion 
    * [] Unticked 


## Parameters

| SAML Custom Connector (Advanced) Field      | Value |
| ----------- | ----------- |
| NameID (fka Email)     | Email       |
| email   | Email `*`       |
| fname   | First Name `*`        |
| lname   | Last Name `*`        |

`*` ☑️ Include in SAML assertion

## Rules

-

## SSO

-

## Acess

Assing it to yourself at least for testing

# Users

-

# Privileges

-


