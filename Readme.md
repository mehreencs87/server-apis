# Auth0's server platforms

[WIP] This is a repository for mapping all supported server platforms by [Auth0](https://auth0.com/)


## Adding a new server api

To add a new `server-api` you need to edit the [index.json](index.json) file and add a new dictionary with the following fields:


- **title**: [`String`] - Display name for the new API doc. Example: `'Server API'`
- **name**: [`String`] - Unique identifier name. Convention adds `-api` string at last if `thirParty == false`. Example: `node-api`, or just `aws` (because it's a `thirdParty` API).
- **url**: [`String`] - Path to the main documentation at https://docs.auth0.com. Example: `/new/server-apis/nodejs` will convert to https://docs.auth0.com/new/server-apis/nodejs.
- **image**: [`String`] - Full url for a representative image. Example: https://auth0.com/platforms-collection/img/php.png.
- **thirdParty**: [`Boolean`] - Wheter is or isn't a 3rd party API. Examples: `aws`, `salesforce`, `firebase`, `wams`, etc.
