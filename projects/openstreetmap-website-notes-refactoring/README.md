# OpenStreetMap-Website: Refactor Notes

The goal of this project is to refactor the existing notes implementation on the OSM website.

* Project: [openstreetmap-website](https://github.com/openstreetmap/openstreetmap-website)
* Related:
  - https://github.com/openstreetmap/openstreetmap-website/issues/3831
  - maybe https://github.com/openstreetmap/openstreetmap-website/pull/3934

The expected deliverable is a mergeable pull request towards https://github.com/openstreetmap/openstreetmap-website. It must at least:
- Follow the idea of a refactoring by changing as little as possible in behaviour and improving the underlying code structure
- Handle the UI part – Map, Forms, Lists, …
- Handle the API part – without any breaking changes to the API
- Handle the Data migration of existing data – discuss details with the operations team
- Handle freatures related to moderation and administration
- Handle special cases for blocked users, hidden or removed notes and similar cases
- Include a wireframe of all proposed UI changes
- Conform to the [CONTRIBUTING.md doc](https://github.com/openstreetmap/openstreetmap-website/blob/master/CONTRIBUTING.md)

## Positive effects of this project

**Remove bugs and improve stability:**

- There are situations when the Notes API returns an error 500 right now. This refactoring will solve the underlying issue. There are multiple issues and even more dupliactes on this topic, eg. https://github.com/openstreetmap/openstreetmap-website/issues/2146.
- It will also solve edgecases like https://github.com/openstreetmap/openstreetmap-website/issues/3396
- It will make the API more stable and easier to handle for data consumers of the API as well. StreetComplete and NotesReview (https://github.com/ENT8R/NotesReview/issues/113) are two apps that reported related problems.
- It will make proposed workarounds obsolete which will make the code simpler and reduce maintance burdens, eg. https://github.com/openstreetmap/openstreetmap-website/pull/3617, https://github.com/openstreetmap/openstreetmap-website/issues/3744, https://github.com/openstreetmap/openstreetmap-website/pull/3607, https://github.com/openstreetmap/openstreetmap-website/pull/3608

**Solid foundation for follow up projects:**

There are multiple issues discussing additions to the notes system. They all require a solid foundation which this project will provide. For example:

- Add a `source` flag to notes and comments to indicate the app or website that created the note/comment, see https://github.com/openstreetmap/openstreetmap-website/issues/3932
- Extend the API for moderation use cases, see https://github.com/openstreetmap/openstreetmap-website/pull/3934
- Update the list-of-notes-UI, see https://github.com/openstreetmap/openstreetmap-website/pull/3386
- Add tags (or similar) to notes, see for example https://github.com/openstreetmap/openstreetmap-website/issues/3932#issuecomment-1440222022
