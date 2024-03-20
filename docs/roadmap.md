# Development Road Map

## Business Case

To replace existing and somewhat dated applications (DutyMan, HalSail), 3rd party Calendar Management tools and manual
process with a single platform that:

* Works consistently across desktop, mobile and web app.
* Shares data so that there is no unnecessary re-entry or import/export
* Supports single sign-on, e.g. Google, Facebook
* Lets user retain control, i.e. the account belongs to them, not their club(s).
* Has "modern" UI patterns

## Beta Test 

A Beta test site is at https://beta.myclub.run

* This is open public Sign Up via email
* Sign Up via Google requires the email address to be pre-approval as the integration is still waiting approval by Google. This will happen towards the end of beta testing.
* The Android App is available on request, as it is not yet published to the App Store. This will happen towards the end of beta testing. 
* The iPhone app will be available shortly of request. As with the Android App it is not yet published to the App Store. 
* All the necessary security is enabled, but until the beta testing is completed please avoid uploading any sensitive or confidential information such as birth dates or bank details   
* Password are one way encrypted to "production" strength as per current recommendations, i.e. resistance to latest hardware

## Issue Tracking 

Public tracking is on [GitHub](https://github.com/blindcatsoftware/myclubdotrun.issues/issues). 

## Release Phases

It is planned to split the development into 3 phases. These phases are for guidance only, as new 
features and enhancement will be continually released.

### Phase 1 - Sailing

Provide core sailing functionality (Calendars, Duties and Results) and enough of the User
and Club Management to manage a full Club trial.

#### Core User Management

* Sign Up
    * Sign Up via Email/Password
    * Sign Up via Gmail (*)
    * Sign Up via FB (^)
    * Sign Up via Apple (^)
    * Sign Up with shared login (for those share a family email) (^)
* Profile
    * Picture *
    * Bio *
    * Preferences (^)
* Account Management
    * Reset Password (*)
    * Close Account (^)
* Club Management
    * User Request to Join Club
    * Club Invites User to Join

#### Core Club Management

* Sign Up
    * Create Club (^) - only inbuilt test clubs at present
    * Create Sandbox (^) - prebuilt set of test user, calendars, duties etc for easy testing
* Account Management
    * Billing (^) - its all free at present
    * Close Account (^)
    * Bulk invite of users (*)
* Member Management
    * Member permissions
    * Club Admin permissions
    * Manage Invites (*)
    * Remove Member (^)
    * Bulk Invite (^)

#### Core Sailing

* Calendar Management
    * Enter sailing and social calendars
    * Use this data for duties and race management
    * Basic Export / import
* Duties
    * Manage Duty Types
    * Manage Duty Templates (rules for a group of Duty Types)
    * Create Duty Rosters by associating Duty Templates to Calendar Entries
    * Duty Rostering
        * User Volunteer
        * User Request Swap
        * Admin Duty Assignment / Reassignment / Cancellation
    * Duty Notification
        * Email notification on any change of status
        * Reminder emails
        * "In app" notifications (^)
    * User Dashboard
        * Visible on home page
        * Duty status and unassigned Duties clearly visible
    * Admin Dashboard
        * Overall allocation status clearly visible (^)
        * Generate "Call to arms" email, i.e. a list of duties that need filling with Volunteer now links (^)
        * Basic reports (^)
        * Basic import / export  (^)
* Race Management
    * Manage Dinghy Types (*)
    * Manage PY Handicaps (*)
    * Manage Fleets (*)
    * Race Results
        * Create Series (*)
        * Create Races within Series (*)
        * Associate Races with Calendar Entries & Duties (*)
        * Race Results
            * "Spreadsheet" style entry of results (*)
            * Automated calculation using handicapping rule (*)
            * Printable Results page (^)
            * Upload of raw race results (^)
            * "Guest" results (i.e. enter results for an unregistered user) (^)
        * Overall results calculator (*)
            * apply series rule, i.e. best 3 count (*)
            * automatic generation of "suggested DNC" based on duty allocation, i.e. no manual extract from Duty Man (*)
    * User Dashboard
        * List of dingies raced (type + sail number) (*)
        * Race result and positions (*)
    * Admin Dashboard
        * Basic import / export (^)
        * PY analysis (^)

#### Platforms

* Web Desktop
* Web Mobile
* Mobile App (*) - limited subset on Android and iPhone

_Note, (^) items are still to be implemented._

_Note, (*) items are partially implemented, i.e. demoable but not complete ._

### Phase 2 - Public Beta

Make the site generally available for a public Beta, extend User functionality to support other Sign Up options
and support outbound email.

At this stage it should be possible to use the site to manage a Club.

#### Legal / Security

* Finalised T&C and privacy policies
* Platform "hardening" (review configs, strong passwords... )

#### Commercial / Billing

* Proposed pricing structure
* No payments necessary during beta phase
* Hopefully have RYA support

#### User Management

* Sign Up
    * Sign Up via Gmail live (i.e. have completed Google's test stage)
    * Sign Up via FB as beta (i.e on request)
    * Sign Up via Apple as beta (i.e on request)
    * Sign Up with shared login (for those share a family email)
    * Accept T&Cs on Sign Up
* Account Management
    * Close Account

#### Club Management

* Sign Up
    * Accept T&C on Sign Up
    * Generation of "sandbox" for quick evaluation
* Membership
    * Membership groups (e.g. sailing, social)

#### Duties

* Import from DutyMan

#### Sailing

* Import from HalSail

#### Web Apps

* Published to App Store (i.e. have completed Google's and Apple's test stage)

#### Email

* Integration with AWS for outbound email
* Ability to bulk sent outbound emails to membership groups

### Phase 3 - Live and Full Club Management

Site is live and making money. Gradually add in more module to cover other aspects of Club Management
based hopefully on feedback. Note that this is currently more a "wish list" than a firm set of requirements.

#### Club Management

* Asset Register
* Training Records
* Membership Subscriptions (but off platform payment)
* Better website integrations, e.g. publishing calendars and events

#### Notifications

* Alternative notifications types
    * SMS
    * Social
* User Notification Dashboard
    * All notifications and emails to a user in once view
* Club Notification Dashboard
    * All notifications and emails to a club in once view, available to Admins

#### Web Apps

* Full In App notifications.
* Better social media integration, e.g. sharing
* Camera integration (scan membership form etc.)





