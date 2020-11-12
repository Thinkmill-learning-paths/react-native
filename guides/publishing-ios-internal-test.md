# Distribute iOS for internal test

This workflow looks like publishing the App to TestFlight.

## Authorisation (once)

Be added as a {company name} iOS Developer.

1. Ask {company name} to be added as an App Developer for the WorryTime iOS App. You will receive an email invitation.

2. Verify that you are added by signing in to [App Store Connect][https://appstoreconnect.apple.com/]. In the top right corner, select your Organisation, and then navigate to the app at My Apps. If you can see the app, you were added.

## Authenticate (once)

1. You must be logged in to Xcode with your Apple ID, Xcode -> Preferences -> Accounts

2. In Xcode's Project Navigator, Select WorryTime Target (left sidebar) and then select Signing and Capabilities Tab (horizontal tabs). Inside Signing, select the team and makes sure "Signing Certificate" is valid.

## Distribute

Publish an app version to TestFlight.

1. Bump the App version, select Project Navigator, then General tab, then at Identity, bump the app version at Version and Build.
2. Ensure "Generic iOS Device" is selected as the Active Scheme. This is found from a drop down at the top of Xcode, where you would toggle between test Device types.
3. You may opt to switch the Build Scheme from Debug to Release, (Product -> Scheme -> Edit Scheme)
4. Create a build (Product -> Build)
5. Create an Archive (Product -> Archive)
6. Once archived the Organizer should open by default (also can be accessed via Window -> Organiser).
7. Inside the Organiser, select the correct build and then click Distribute App, continue with all of the defaults
8. Once this is complete, the app will appear by itself in TestFlight after a short period of time.

## Invite stakeholders to TestFlight (once)

1. In App Store Connect at ["Users and Access"](https://appstoreconnect.apple.com/access/users), first add them as a Developer for the App. Make sure to invite them using the email they use to log in to the App Store on the device which they want to test from (if that device is their personal phone, this will probably be their personal email).

2. They must then go ahead and accept the Invitation.

3. Invite them to go ahead and download TestFlight app from the App Store.

4. In App Store Connect at "My Apps", navigate in to the WorryTime app.

5. Click the tab TestFlight tab, then All Testers, add individuals to TestFlight Testers. They will receive a TestFlight invitation email.

6. Once all of this is valid and accepted, they will gain access to test builds via the TestFlight app which they have downloaded.
