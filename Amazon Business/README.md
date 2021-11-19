## Amazon Business

N.B I've left this as *.co.uk* so replace whatever domain you need.

- Add App
- SAML Custom Connector (Advanced)

### Info
- Amazon Business (Country)

### Configuration

- Audience (EntityID) - https://www.amazon.co.uk
- Recipient - https://www.amazon.co.uk/bb/feature/sso/action/3p_redirect?idpId=<theid in the Amazon SSO Settings>
- ACS (Consumer) URL Validator*
 - ^https:\/\/www\.amazon\.co\.uk\/bb\/feature\/sso\/action\/3p_redirect$

- ACS (Consumer) URL*
 - https://www.amazon.co.uk/bb/feature/sso/action/3p_redirect?idpId=<theid in the Amazon SSO Settings>

- Login URL
 - https://www.amazon.co.uk/bb/feature/sso/action/3p_redirect?idpId=<theid in the Amazon SSO Settings>

- SAML initiater
 - OneLogin

- SAML nameID format
 - Unspecified

- SAML signature element
 - Assertion

- Encryption assertion 
 - Unticked 


## Parameters

