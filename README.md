# ![LOGO](logo.png) Azure Reservation **flow**ground Connector

## Description

A generated **flow**ground connector for the Azure Reservation API (version 2018-06-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/reservations/2018-06-01/swagger.json<br/>
Generated at: 2019-05-07T17:38:44+03:00

## API Description

This API describe Azure Reservation

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Get operations.

> List all the operations.

*Tags:* `Operation`

#### Input Parameters
* `api-version` - _required_ - Supported version.

### Get all `ReservationOrder`s.

> List of all the `ReservationOrder`s that the user has access to in the current tenant.

*Tags:* `Reservation`

#### Input Parameters
* `api-version` - _required_ - Supported version.

### Get a specific `ReservationOrder`.

> Get the details of the `ReservationOrder`.

*Tags:* `Reservation`

#### Input Parameters
* `reservationOrderId` - _required_ - Order Id of the reservation

* `api-version` - _required_ - Supported version.

### Merges two `Reservation`s.

> Merge the specified `Reservation`s into a new `Reservation`. The two `Reservation`s being merged must have same properties.

*Tags:* `Reservation, Merge`

#### Input Parameters
* `reservationOrderId` - _required_ - Order Id of the reservation

* `api-version` - _required_ - Supported version.

### Get `Reservation`s in a given reservation Order

> List `Reservation`s within a single `ReservationOrder`.

*Tags:* `Reservation`

#### Input Parameters
* `reservationOrderId` - _required_ - Order Id of the reservation

* `api-version` - _required_ - Supported version.

### Get `Reservation` details.

> Get specific `Reservation` details.

*Tags:* `Reservation`

#### Input Parameters
* `reservationId` - _required_ - Id of the Reservation Item
* `reservationOrderId` - _required_ - Order Id of the reservation

* `api-version` - _required_ - Supported version.

### Updates a `Reservation`.

> Updates the applied scopes of the `Reservation`.

*Tags:* `Reservation` `ApplyScope`

#### Input Parameters
* `reservationOrderId` - _required_ - Order Id of the reservation

* `reservationId` - _required_ - Id of the Reservation Item
* `api-version` - _required_ - Supported version.

### Get `Reservation` revisions.

> List of all the revisions for the `Reservation`.

*Tags:* `Reservation`

#### Input Parameters
* `reservationId` - _required_ - Id of the Reservation Item
* `reservationOrderId` - _required_ - Order Id of the reservation

* `api-version` - _required_ - Supported version.

### Split the `Reservation`.

> Split a `Reservation` into two `Reservation`s with specified quantity distribution.

*Tags:* `Reservation, Split`

#### Input Parameters
* `reservationOrderId` - _required_ - Order Id of the reservation

* `api-version` - _required_ - Supported version.

### Get list of applicable `Reservation`s.

> Get applicable `Reservation`s that are applied to this subscription.

*Tags:* `AppliedReservation`

#### Input Parameters
* `api-version` - _required_ - Supported version.
* `subscriptionId` - _required_ - Id of the subscription

### Get the regions and skus that are available for RI purchase for the specified Azure subscription.

*Tags:* `Catalog`

#### Input Parameters
* `api-version` - _required_ - Supported version.
* `subscriptionId` - _required_ - Id of the subscription
* `reservedResourceType` - _required_ - The type of the resource for which the skus should be provided.
* `location` - _optional_ - Filters the skus based on the location specified in this parameter. This can be an azure region or global

## License

**flow**ground :- Telekom iPaaS / azure-com-reservations-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
