# modernization
Initial work on building out a case for Modernization of the tooling the Node.js org uses.

We currently have a suite of automation tooling. That said, this tooling could certainly be enhanced... especially with more modern GitHub features like Apps, Actions, and the [Probot](https://probot.github.io/) framework being worked on actively. Node.js is a first-class citizen in all of the newer tooling that GitHub has released, so it makes sense for us to Use the Platform™ that is using what we're building.

## Current Automation:

**Release:**
- Steps to release a version of Node.js (https://github.com/nodejs/node/blob/master/doc/releases.md)
- Steps to promote a version of Node.js to LTS.

**nodejs/node:**
- Commenting that a CI build is running
- CI checks
- Canary in the Gold Mine (is this actually being used in tests/checks?)

**Org-wide:**
- Meeting issue creation
  - https://github.com/nodejs/make-node-meeting
  - https://github.com/nodejs/meeting-picker
  - https://github.com/nodejs/node-meeting-agenda
  - https://github.com/nodejs/create-node-meeting-artifacts

## Missing Automation:
- Teams and `README.md`
  - Currently this is a fully manual process
  - Both addition and removal from teams and `README.md` is manual.
- Automatic labeling
  - In nodejs/node we could be automatically labeling based off of the `Subsystem`, `Platform`, and `Version` parts of the issue template.
  - Additionally, other repositories could opt-into auto-labeling via detected possibilities.
- Fast-track requesting in nodejs/node
  - Enable a contributor to opt-in a PR to being fast-tracked
  - Automagically link CI lite
- Automatically PR meeting minutes
  - Could pull content the same way we push it into a doc, use a markdown linter with `--fix` and submit a PR for reivew. Removes the burnen from intidivudal contributors.
