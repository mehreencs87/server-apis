# Auth0's server platforms

[WIP] This is a repository for mapping all supported server platforms by [Auth0](https://auth0.com/)


## Adding a new server api

To add a new `server-api` you need to edit the [index.json](index.json) file and add a new dictionary with the following fields:


- **title**: [`String`] - Display name for the new API doc. Example: `'Server API'`
- **name**: [`String`] - Unique identifier name. Convention adds `-api` string at last if `thirParty == false`. Example: `node-api`, or just `aws` (because it's a `thirdParty` API).
- **url**: [`String`] - Path to the main documentation at https://docs.auth0.com. Example: `/new/server-apis/nodejs` will convert to https://docs.auth0.com/new/server-apis/nodejs.
- **image**: [`String`] - Full url for a representative image. Example: https://auth0.com/platforms-collection/img/php.png.
- **thirdParty**: [`Boolean`] - Wheter is or isn't a 3rd party API. Examples: `aws`, `salesforce`, `firebase`, `wams`, etc.


## Release

Make sure you have [bump](https://github.com/ianstormtaylor/bump) and [git-extras](https://github.com/tj/git-extras)
Follow the next steps:

``` bash
  # Once finished your changes and commit them, run:
  bump {patch,minor,major,VERSION}

  # Then create the changelog for the release, using
  # the retrieved version by last command:
  git changelog --tag <version>

  # Then, just run:
  git add . && git release <version>

  # Done!
```
## Issue Reporting

If you have found a bug or if you have a feature request, please report them at this repository issues section. Please do not report security vulnerabilities on the public GitHub issue tracker. The [Responsible Disclosure Program](https://auth0.com/whitehat) details the procedure for disclosing security issues.

## Author

[Auth0](auth0.com)

## License

This project is licensed under the MIT license. See the [LICENSE](LICENSE) file for more info.
