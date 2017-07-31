Import react-relay/classic or react-relay.

For use in libraries that want to support both react-relay and react-relay
modern.

Just add:

```json
{
  "peerDependencies": {
    "react-relay-compat": "^0 || ^1"
  }
}
```

And import:

```js
const RelayClassic = require('react-relay-compat');
// or
const MaybeRelayModern = require('react-relay-compat/modern');

if (MaybeRelayModern) {
  const RelayModern = MaybeRelayModern;
  ...
}
```
