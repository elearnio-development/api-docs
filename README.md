# api-docs
## elearnio API documentation

### authentication

to be discussed

### get /members

Supported filter:
* role
* fullname
* member.id
* email
* employee_id
* group.external_id
* group.id

Additional notes:
* member.groups[] accepts group.external_id

### patch /members

v1 does not allow an update of:
* email
* role

Additional notes:
* when updating groups, always send all groups

### get /groups

Supported filter:
* id
* name
* external_id

