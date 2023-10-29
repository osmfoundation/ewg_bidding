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

**Remove bugs, improve stability and reduce maintenance burden:**

For example:

- An issue about notes without comments https://github.com/openstreetmap/openstreetmap-website/issues/2146
- Another issue related to notes without comments https://github.com/openstreetmap/openstreetmap-website/issues/3396
- https://github.com/openstreetmap/openstreetmap-website/issues/3744 is waiting on the refactoring before being reviewed
- Multiple pull request can be closed which are workarounds for the current implementation. For example https://github.com/openstreetmap/openstreetmap-website/pull/3617, https://github.com/openstreetmap/openstreetmap-website/pull/3607, https://github.com/openstreetmap/openstreetmap-website/pull/3608

**Solid foundation for follow up projects:**

There are multiple issues discussing additions to the notes system. They all require a solid foundation which this project will provide. For example:

- Improve notes/comments with an optional information on the app or website that created the note/comment, see https://github.com/openstreetmap/openstreetmap-website/issues/3932
- Extend the API for moderation use cases, see https://github.com/openstreetmap/openstreetmap-website/pull/3934
- Update the list-of-notes-UI, see https://github.com/openstreetmap/openstreetmap-website/pull/3386
- Add tags (or similar) to notes, see for example https://github.com/openstreetmap/openstreetmap-website/issues/3932#issuecomment-1440222022
