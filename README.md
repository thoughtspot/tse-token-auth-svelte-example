# Example Trusted Authentication (in Svelte)

This repository contains an example of using trusted authentication.  It's written using Svelte and SvelteKit, but the concepts should be applicable to any framework.

The APIs provided are:

* `GET /token?user=<username>` - gets an auth token for the specified user
* `GET /env` - returns the environment variables that are used for the auth token.  This is mostly just to verify the settings.  Note that only part of the secret key is returned.

To run this example, you need to provide the following environment variables:
* TS_URL - the URL of your ThoughtSpot Server.
* ORG_ID - the ID of the organization to use.  Use 0 if for the primary org.
* TS_SECRETKEY - the secret key to use for getting the auth token.
