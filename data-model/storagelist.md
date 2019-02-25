# storage list

## common-data

Account-shared data of this service.

store at: cloud datastore, namespace is ``default`'

includes:
- user-data (auth, permissions)
- master data
and so on


## account-data

Account-oriented data of this service.

store at: cloud datastore, namespace is tenant-id (AccountId)

includes:
- somthing
and so on
