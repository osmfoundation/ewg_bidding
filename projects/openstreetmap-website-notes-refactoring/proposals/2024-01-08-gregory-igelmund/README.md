# Proposal to implement the Notes Refactoring

## About the author

I've been working on Rails web applications since 2011, freelancing as a Rails developer since 2016. I will perform 100% of the implementation work outlined in this proposal.

I've implemented a previous project (the [User Mute feature](..projects/ability-to-mute-other-users)).


## Refactoring guidelines

Generally the refactoring should:

- fix the underlying technical problems leading to the bugs described in the following issues:
  - <https://github.com/openstreetmap/openstreetmap-website/pull/3617>
  - <https://github.com/openstreetmap/openstreetmap-website/pull/3607>
  - <https://github.com/openstreetmap/openstreetmap-website/pull/3608>
- not change any other behaviour than the undesired buggy behaviour described in the linked issues above
- not cause any extra work for the operations team or the project maintainers for the duration of the data migration

### Refactoring plan

Andy Allan describes [here](https://github.com/openstreetmap/openstreetmap-website/issues/3831#issue-1482565414) the technical issues in detail and also provided [here](https://github.com/openstreetmap/openstreetmap-website/issues/3831#issuecomment-1341562044) a step-by-step plan on how to address the situation.

I agree with the action plan described by Allan and therefore would simply follow these general steps. Further needs for the refactoring and any clarification of the implementation details will be discussed and coordinated with the OSM website maintainers and community.


## Time effort and costs

I estimate that I'll have to spend between 3 to 6 days of 8h working days into implementation work, communication with the operations team, cleaning up after the successful data migration, updating documentation and tests etc.