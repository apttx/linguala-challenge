# Linguala Challenge

We're a small startup and always looking for people to help us build a web-platform all about language services. This repo is an easy way to show off what you know & what you've learned.

## Stack

We use Node (Koa), GraphQL (Apollo), MongoDB & React with Gatsby and would like you to use the same. DB isn't as important; if you know your way around something else, that's fine here, too.

## Challenge

We've got three topics we're currently working on:
- User authentication via identity providers
- Translator profiles (via GraphQL)
- Web app to display & interact with everything

You don't have to know all of this. Pick the one you're familiar with & mock the rest as you need it.

### User authentication

We'd like to separate users from resources. We currently use Keycloak as an identity provider & user management system, but feel free to use something else you think is better. On the resource side, we use Passport as a pluggable authentication framework.

#### Tasks

- Set up a Koa server
- Set up Passport middleware that
  - parses a bearer JWT from the Authorization header
  - reads a user from the database & returns it to Passport to put into `ctx.state`
  - allows requests that don't have the Authorization header set & just leaves `ctx.state.user` unset
- Add an endpoint that returns the logged in user, if available

Some suggestions:
- Use Postman, Insomnia or the like for easy request development
