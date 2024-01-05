## Mute other users (completed)

> [!NOTE]
> This project [was completed](https://github.com/openstreetmap/openstreetmap-website/pull/4284) and is live on openstreetmap.org

---

Users who receive unwanted messages to their [openstreetmap.org message inbox](https://www.openstreetmap.org/messages/inbox) currently have to report the message writer and wait for an administrator to take action. The OpenStreetMap website should make it possible for anyone to painlessly mute (ignore) private messages from another user.

* Project: [openstreetmap-website](https://github.com/openstreetmap/openstreetmap-website)
* Related:
  - https://github.com/openstreetmap/openstreetmap-website/issues/3129
  - https://community.openstreetmap.org/t/rfc-on-engineering-working-group-project/1542

The expected deliverable is a mergeable pull request towards https://github.com/openstreetmap/openstreetmap-website. It must at least:
- not display messages sent from user A in user B's inbox if user B has muted user A (this includes messages sent by responding to email notifications)
- not show any message notifications to a user from a muted user, including email notifications sent alongside messages
- otherwise preserve existing notification functionality for changesets, notes, diaries, etc.
- comprise a UI such that a user can view and change which users they have muted
- not allow admins and moderators to be muted
- declare the business logic how past and future messages are handled in both the Inbox UI and the data model in case of muting and unmuting
- include a wireframe of all proposed UI changes
- conform to the CONTRIBUTING.md doc [here](https://github.com/openstreetmap/openstreetmap-website/blob/master/CONTRIBUTING.md)

