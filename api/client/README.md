### What is the significance of client package ?

- This package deals with http client related implementations.
- This also implements the stuff that deals with usage of client on terminal console.

### Important Notes:

- cli.go defines the generic client settings, e.g. it includes:
  - config,
  - server i.e. host information,
  - stdout, stderr, stdin,
  - certificates to communicate with server
- cli.go can be treated as very generic helper utility
- commands.go maps the openebs specific commands to their handlers in client.
- Each folder relates to an entity w.r.t. openebs
  - This entity implements the client side logic
  - Technically this is the http client side implementation of the entity.
