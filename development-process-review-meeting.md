# Development Process Review Meeting

These notes are captured as a part of the review of the software development life cycle @ 365.

## Process

### New Feature

1. Requests Come In as a proposal
     1. Usually goes through a few iterations of requirements gathering.
     1. Estimating items first.
     1. Add priorities
         1. Ryan works with the business to determine the priority.
1. Logged in the backlog
1. Backlog grooming/developer Capacity
1. Work
    1. Dev Test
    1. Sometimes leveraging the local dev machine for testing.
    1. Pull request
        1. One person approves back to the develop branch.
1. Deployment
    1. Dev Environment Deploy (based on branch name convention)
        1. Typically branched off a feature branch.
    1. Staging/UAT
        1. Deployed from the develop.
    1. Production
        1. From master off of a Tag.

### Bug Fixes

1. Bugs are reported.
     1. Generally reported through Jira (Alex and Justina)
     1. Not really reported with Steps to reproduce
     1. Investigation of the issue and then assigned Priority
1. Logged in the backlog
1. Assigned based on priority.
1. Work
    1. Dev Test
    1. Sometimes leveraging the local dev machine for testing.
    1. Pull request
        1. One person approves back to the develop branch.
1. Deployment
    1. Dev Environment Deploy (based on branch name convention)
        1. Typically branched off a feature branch.
    1. Staging/UAT
        1. Deployed from the develop.
    1. Production
        1. From master off of a Tag.

### Internal Work

1. Must have an approved date and approved by

### TDR

TDRs are essentially a catchall category for left over work and bugs that need a resolution.
Almost all the TDR items are created by the dev team.
    Business is always requiring development and deployment.

### Backlog Grooming Sessions

1. How often are grooming sessions.
1. Prioritization of work items here.
1. during stand ups assess available time for developers.

### Confluence

<http://confluence.signs365.local:8090/pages/viewpage.action?pageId=10588353>

- SD - Service Desk - all the requirements from the business to fix right now.
- Prioritized - what's the most important.
- APD - Agile Product Development

# Pain Points

1. UAT
    1. Limited capacity in testing in amount and velocity.
1. Only 1 imaging environment
    1. It is a bottleneck on only because its one item per deployment
1. Capacity of Jonathan
    1. at least once a month. The items that are impacted by infrastructure are larger items
1. Communication strategy between business and IT.
1. ImageProcessing for Reprints -