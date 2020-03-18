**Bug Fixes**:

- Address dc population bug where there was a 500 error if you had a dc string that included a space.

**New Operations**:

- Get a list of objects created or modified by a user with audit_responsibility.  See docs for more details.
- Update solr with gsearch with update_solr.  See docs for more details.

**New Fedora Public Methods**:

- FedoraRequest.audit_responsibility(username): Returns a list of objects where a specific username has created or modified the object at some point.
- FedoraRequest.update_solr_with_gsearch(): Attempts to update solr documents and returns a Message with successes, errors, and attempts.