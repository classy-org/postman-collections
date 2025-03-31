# GoFundMe Pro API Postman Collections

## Overview

This repository contains Postman collections that the GoFundMe Pro team has put together to showcase the functionality of the GoFundMe Pro API. To get the most out of this collection, ensure that you have [Postman downloaded](https://www.postman.com/downloads/) and installed.

## Importing Collections

To use these collections, you'll need to import them into your own workspace. You can follow the steps in [this tutorial video from Postman](https://youtu.be/KdaiVdNMgL4?si=L4531gLnHO3qoQb0&t=103) to see how to import the collection -- along with environment variables -- to your Postman workspace.

## Environments

Each collection will have one or more environments. These environments contain variables that you'll need to define in the UI. Commonly, those will be:

- **GoFundMe Pro API credentials**, like Client ID and Client Secret
- **IDs to records** contained in your GoFundMe Pro organization that you will be fetching via Postman

Some environment variables may be used by the collection itself to set values that other requests in the collection need. If in doubt, refer to each collection's documentation or `README` included in the collection's folder for more information.

## Important Environment Considerations

As you enter the data needed to connect to GoFundMe Pro, please be considerate of how you enter your `client_id` and `client_secret`! **These values should be treated with the same sensitivity as your password!** If someone gets this data that shouldn't have it, they can make any request as though they were you! To protect yourself, ensure that you do the following:

- Whenever you add data to the Postman environment variables, only do it in the `Current Value` column
  - Please review [this Postman documentation](https://learning.postman.com/docs/sending-requests/variables/variables/#initial-and-current-values) to understand the difference between Initial and Current values
- Do not enter your client id and secret into any field that does not have the `secret` type
  - Please review [this Postman documentation](https://learning.postman.com/docs/sending-requests/variables/variables/#variable-types) to understand the difference between types

### Multiple Environments

Some collections may have more than one environment. Ensure that you read the documentation to understand what each environment's purpose is. In some cases, we provide a mock server through Postman that simulates a response from the API without requiring credentials. The mock server can be used outside of Postman, but will only behave properly if you use the requests contained in the collection. For more information on mock servers, please review [this Postman documentation](https://learning.postman.com/docs/designing-and-developing-your-api/mocking-data/setting-up-mock/).
