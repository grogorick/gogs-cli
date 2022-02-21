# Gogs command line interface

Interact with Gogs servers via *curl* requests to their [REST API v1](https://github.com/gogs/docs-api).

Use `./gogs` to show available actions.  
Use `./gogs <action>` to show required parameters.  
Use `./gogs <action> <argument> ...` to run actions.

## Available actions include to
- create/delete/list/query user/organization **repositories**
- add/remove/list repository **collaborators**
- create/list organization **teams**
- add/remove/list organization **team members**
- add/remove organization **team repositories**
- fetch **raw** file content

## Setup
- Gogs server URL
    - Required in the form `https://try.gogs.io`
    - Via environment variable or file in this directory
- Gogs API token
    - Create at `https://YOUR.GOGS.SERVER/user/settings/applications`
    - Via environment variable or file in this directory

(See `config` section in `./gogs`)

---

*The REST API does not yet allow some actions (like organization team deletion).  
Similarly, this cli does not cover all avilable actions &mdash; pull requests are welcome!*
