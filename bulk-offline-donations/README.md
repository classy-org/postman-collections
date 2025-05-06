# Bulk Offline Donations

## Purpose

This collection showcases two strategies for using a Postman runner in order to sync offline donations onto the GoFundMe Pro platform

## How To Use

If you don't have experience with Postman, please take a look at their Getting Started documentation! <https://learning.postman.com/docs/getting-started/overview/>
This collection is meant to be a playground, allowing you to use either a Mock Server or your own GoFundMe Pro Account. You'll need to follow steps to get API credentials through GoFundMe Pro: <https://support.classy.org/s/article/intro-to-the-classy-api>

## Using the Mock Server

If you either don't have GoFundMe Pro credentials, or would prefer to not make these calls against your account, you can leverage a Mock Server we've put together as part of this collection. The mock server bases its responses on the Examples we've provided under each request, using a mixture of hard-coded data and faked data to mimic executing requests against the API. You can use this mock server to freely try out these requests. It doesn't perform any authentication, and functions outside the context of Postman. So you can try out these calls against the mock server using cURL, or the language of your choice, to try it out! To use the mock server, ensure you are using the GoFundMe Pro API Mock Server environment!

## Using the GoFundMe Pro API

If you are using your GoFundMe Pro Account, ensure you have your Client ID and Client Secret from GoFundMe Pro. If you don't have these or don't know how to get them, you can find that information from this support article: <https://support.classy.org/s/article/intro-to-the-classy-api>

Once you have these, ensure you are using the GoFundMe Pro API environment, and enter the Client ID and Client Secret into the 'current value' field for client_id and client_secret respectively.
Before making any of the donation requests you'll need to authenticate with the API. To do so, use the App Auth request under the Authentication folder. This will make a call to the API, and assuming you have working credentials will provide a token that will be automatically saved and used for subsequent requests. These tokens have a limited timeframe in which they are valid, so if you start seeing errors that you have an invalid token, simply run the App Auth request again to get a new token.

Once you have this token, you should be ready to start sending requests to the GoFundMe Pro API and syncing offline donations into your campaigns.

**NOTE: Running these requests to add offline donations will permanently add transaction data to your organization and campaigns. Organizations using this collection as well as the GoFundMe Pro API generally are solely responsible for managing imported data and ensuring data accuracy. GoFundMe Pro recommends that you exercise caution when utilizing this collection and ensure that you truly mean to add offline donations before proceeding.**
