### User authentication challenge

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
