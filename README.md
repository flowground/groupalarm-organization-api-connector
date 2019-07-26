# ![LOGO](logo.png) groupalarm Organization API **flow**ground Connector

## Description

A generated **flow**ground connector for the groupalarm Organization API API (version 1.15.3).

Generated from: https://app.groupalarm.com/api/v1<br/>
Generated at: 2019-07-26T13:59:34+03:00

## API Description

The organization service implements a the organization logic in GroupAlarm.<br/>
<br/>
# Authentication<br/>
<br/>
<!-- ReDoc-Inject: <security-definitions> --><br/>

## Authorization

Supported authorization schemes:
- API Key
- API Key

## Actions

### UpdateOrganization
> Update an existing organization with passed organization payload<br/>

*Tags:* `organization`

### CreateOrganization
> Create an organization with passed organization payload<br/>

*Tags:* `organization`

### GetOrganization
> Get specific organization by its ID<br/>

*Tags:* `organization`

#### Input Parameters
* `organizationID` - _required_ - id of the requested organization<br/>

### GetChildren
> Get paginated children of specific organization by its ID<br/>

*Tags:* `children`

#### Input Parameters
* `organizationID` - _required_ - id of the requested organization<br/>
* `limit` - _optional_ - max. amount of entries in list<br/>
* `offset` - _optional_ - amount of entries to skip<br/>

### GetOwnerInParentOrganization
> Gets the topmost parent organization the given user is the owner of<br/>

*Tags:* `owner`

#### Input Parameters
* `organizationID` - _required_ - id of the organization<br/>
* `userID` - _required_ - id of the user<br/>

### AddOwner
> Update an existing organization by adding a new owner<br/>

*Tags:* `owner`

#### Input Parameters
* `organizationID` - _required_ - id of the organization<br/>
* `userID` - _required_ - id of the user<br/>

### RemoveOwner
> Update an existing organization by removing an existing owner<br/>

*Tags:* `owner`

#### Input Parameters
* `organizationID` - _required_ - id of the organization<br/>
* `userID` - _required_ - id of the user<br/>

### GetOwnedOrganizations
> Get all organizations for user in JWT token where the user is the owner of<br/>

*Tags:* `organizationsByOwner`

### GetPaginatedOrganizations
> Get paginated organizations for user with the passed JWT token<br/>

*Tags:* `organizations`

#### Input Parameters
* `limit` - _optional_ - max. amount of entries in list<br/>
* `offset` - _optional_ - amount of entries to skip<br/>

## License

**flow**ground :- Telekom iPaaS / groupalarm-organization-api-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
