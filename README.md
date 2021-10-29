# api-docs
## elearnio API documentation

### authentication

* header param: user_api_key

### get /members

Supported filter:
* role
* full_name
* id (of member)
* email
* employee_id
* external_id (of group)
* group_id (of group)

Additional notes:
* member.groups[] accepts external_id (of group)

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
