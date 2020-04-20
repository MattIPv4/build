# StatusPage

This document relates to the [StatusPage](https://www.statuspage.io/) for Node.js, which can be
found at [status.nodejs.org](https://status.nodejs.org).

## Access

The following people have access to the StatusPage control panel. New accounts can be added via the
[User Management](https://manage.statuspage.io/organizations/m3074zj4qnr9/team) page.

Access to StatusPage is unrestricted, so anyone in this list can make changes to the styling of
the page, change what components are listed, see who is subscribed to notifications (PII: emails,
phone numbers) and manage incidents on the page.

The only additional "permission" is that one email address is considered the owner of the
status page. This account cannot be removed by other members and acts as the official owner of the
page for communication with the StatusPage folks if needed.

| GitHub                                         | Email (for StatusPage access)  | Role   |
|------------------------------------------------|--------------------------------|--------|
| [@MattIPv4](https://github.com/MattIPv4)       | nodejs-status@mattcowley.co.uk | Owner  |
| [@brianwarner](https://github.com/brianwarner) | operations@openjsf.org         | Member |

## Twitter

There is also a Twitter account, [@NodejsStatus](https://twitter.com/NodejsStatus), for the
status page.

This account is run by [@MattIPv4](https://github.com/MattIPv4) via nodejs-status@mattcowley.co.uk,
but is added to the [Twitter integration](https://manage.statuspage.io/pages/rxy2rhgm8q1n/twitter)
on StatusPage and will automatically tweet any incidents created on the page.

## Customisations

The [statuspage](../statuspage) directory in this repository contains a backup of the major
customisations applied to the Node.js status page. These should be updated whenever the
customisations are changed on the status page.

[colors.md](../statuspage/colors.md) contains the custom color set for the whole status page
(including emails for subscribers) in
[Your Page > Customize page and emails > Colors](https://manage.statuspage.io/pages/rxy2rhgm8q1n/design#colors-container).

[styles.scss](../statuspage/styles.scss) stores the custom styling that is applied to all web pages
of the Node.js StatusPage site. This is controlled from the
[Customize HTML & CSS](https://manage.statuspage.io/pages/rxy2rhgm8q1n/full-customize) view
accessed from the button top-right on
[Your Page > Customize page and emails > Customize status page](https://manage.statuspage.io/pages/rxy2rhgm8q1n/design#design-container).

[header.html](../statuspage/header.html) contains the custom HTML used for the header on the
status page. It is important to note that this replaces the default header (logo & subscribe
button), so using this should be avoided if possible. Like the custom styling, this is managed from
the [Customize HTML & CSS](https://manage.statuspage.io/pages/rxy2rhgm8q1n/full-customize) page.

[footer.html](../statuspage/footer.html) contains custom HTML injected into the footer of the
status page website. This doesn't replace any default content and is a good place for custom
scripting if needed. This is also controlled from the
[Customize HTML & CSS](https://manage.statuspage.io/pages/rxy2rhgm8q1n/full-customize) page.
