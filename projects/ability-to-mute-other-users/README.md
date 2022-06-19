## Mute other users

Users who receive unwanted messages currently have to report the message writer and wait for an administrator to take action. The OpenStreetMap website should make it possible for anyone to painlessly mute (ignore) private messages (but not comments on changesets) from another user.

* Project: [openstreetmap-website](https://github.com/openstreetmap/openstreetmap-website)
* Related issues:
  - https://github.com/openstreetmap/openstreetmap-website/issues/3129
  - https://github.com/openstreetmap/openstreetmap-website/issues/3129#issuecomment-801239631
  - https://lists.openstreetmap.org/pipermail/dev/2018-September/030383.html

The expected deliverable is a mergeable pull request towards https://github.com/openstreetmap/openstreetmap-website. It must at least
- have a list per user of the other muted users based on their user ids in the database
- must not show in the inbox of a user any message from a user whose user id is on the blacklist
- comprise a UI such that a user can see and change which users they have muted (by user id and current user name)
- declare the business logic how past and future messages are handled in both the Inbox UI and the data model in cases of muting and unmuting
- cover the intended functionality and all control flow paths by tests

The "report" mechanism mentioned in the Github issue is out of scope in this tender.
