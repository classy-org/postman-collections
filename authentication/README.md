# Authentication Example

## Purpose

The Classy API offers extensive functionality when trying to fetch data. This collection offers a starting point to view how credentials are exchanged for an access token that unlocks access to the rest of our public API.

This collection will not modify any data in your account or actually exchange your credentials for an access token from our service. It utilizes Postman's Mock Server feature to simply provide a framework of understanding to build from.

More information on how to use the Mock Server is [further down in this README](#mock-server).

## How Do I Use This

If you don't have experience with Postman, please take a look at their [Getting Started documentation!](https://learning.postman.com/docs/getting-started/overview/)

This collection is meant to be a playground, allowing you to use a Mock Server as a visual aid to understand how our authentication process works. Our other public collections include this authentication endpoint and set the access token returned from a succesful request as a bearer token in the Authorization header for subsequent requests to other endpoints. You'll need to follow the steps to get API credentials through Classy Manager as outlined [here.](https://support.classy.org/s/article/intro-to-the-classy-api)

For instructions on how to import this collection and environment variables, refer to the README.md file at the root of this repository.

Once this collection has been imported into your workspace, please refer to the documentation contained within to understand what calls to make.

## Mock Server

If you either don't have Classy credentials, or would prefer to not make these calls against your account, you can leverage a Mock Server we've put together as part of this collection. The mock server bases its responses on the Examples we've provided under each request, using a mixture of hard-coded data and faked data to mimic executing requests against the API. You can use this mock server to freely try out these requests.

The mock server provides a faker implementation of how you would normally interact with our service to exchange your credentials for an access token as well as common errors you might see when doing so. To leverage this feature, ensure you import and use the `Authentication Mock Server` environment!
