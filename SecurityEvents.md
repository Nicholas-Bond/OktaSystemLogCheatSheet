# Okta Event Types of Interest for Security Teams

## User Events

|EventType Filter|Notes|
|------------- |-------------|
|eventType eq "user.session.start"|User logging in|
|eventType eq "user.session.end"|User logging out|
|eventType eq “policy.evaluate_sign_on”|Sign in policy evaluation|
|eventType eq “user.account.lock”|Okta user locked out|
|eventType sw "user.authentication.auth"|All types of Auth events, covering MFA, AD, Radius, etc|
|eventType eq "user.account.update_password"|User changing password|
|eventType eq "user.authentication.sso"|User accesing app via single sign on|
|eventType eq "user.authentication.auth_via_mfa"|MFA challenge|
|eventType eq "user.mfa.factor.update"|User changing MFA factors|

## Okta Events

| EventType Filter |  Notes|
| ------------- | -------------|
|eventType eq "user.session.access_admin_app | These events are associated with users accessing the Admin section of your Okta instance |
|eventType eq "user.account.reset_password" | User password reset by Okta Admin |
|eventType eq "zone.update"|Modification of a Network Zone|
|eventType eq "user.account.privilege.grant"|Granting Okta Admin to a user|
|eventType eq "group.user_membership.add"|Adding Okta user to a group|
|eventType eq "application.user_membership.add"|Adding user to application membership|
|eventType eq "policy.lifecycle.create"|Creation of a new Okta Policy|
|eventType eq ”application.lifecycle.create”|New Application created|
|eventType eq ”user.lifecycle.activate”|New Okta user|
|eventType eq "application.provision.user.push"|Assign application to user|
|eventType eq ”user.lifecycle.deactivate”|Deactivate Okta user|
|eventType eq ”user.lifecycle.suspend”|Suspend Okta user|
|eventType eq "user.session.clear"|Okta user login session cleared|
|eventType eq "system.api_token.create"|Creation of a new Okta API token|
|eventType eq “system.org.rate_limit.violation”|Hitting the rate limit on requests|
|eventType eq “user.mfa.factor.deactivate”|Removed MFA factor from user|
|eventType eq "user.mfa.factor.reset_all"|Remove all MFA factors from user|
