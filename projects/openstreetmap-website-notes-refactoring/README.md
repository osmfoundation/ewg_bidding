# OpenStreetMap-Website: Refactor Notes

The goal of this project is to refactor the existing notes implementation on the OSM website.

* Project: [openstreetmap-website](https://github.com/openstreetmap/openstreetmap-website)
* Related:
  - https://github.com/openstreetmap/openstreetmap-website/issues/3831
  - maybe https://github.com/openstreetmap/openstreetmap-website/pull/3934

The expected deliverable is a mergeable pull request towards https://github.com/openstreetmap/openstreetmap-website. It must at least:
- Follow the idea of a refactoring by changing as little as reasonable by improving the underlying code structure
- Handle the UI part – Map, Forms, Lists, …
- Handle the API part – without any breaking changes to the API
- Handle the Data migration of existing data – discuss details with the operations team
- Handle freatures related to moderation and administration
- Handle special cases for blocked users, hidden or removed notes and similar cases
- Include a wireframe of all proposed UI changes
- Conform to the [CONTRIBUTING.md doc](https://github.com/openstreetmap/openstreetmap-website/blob/master/CONTRIBUTING.md)

## Side effects

A side effect of this refactoring will be that a recurring error 500 will not be possible anymore, see https://github.com/openstreetmap/openstreetmap-website/issues/2146 for more.

## Possible follow up projects

This refactoring will unblock follow possible follow up improvements to the website and api that are not being worked on ATM due to the outdated foundation of the notes system.

For example:

- Add a `source` flag to notes and comments to indicate the app or website that created the note/comment, see https://github.com/openstreetmap/openstreetmap-website/issues/3932
- Update the notes UI, related to https://github.com/openstreetmap/openstreetmap-website/pull/3386
