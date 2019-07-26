# master
- Fix bugs with `ConnectionHandler` bindings not working.
- Add bindings for getting and setting arrays of primitives as values on `RecordProxy`.
- Move from data-last to data-first to better adhere to what BuckleScript is pushing.
- Add `ReasonRelayUtils` module with helpers for dealing with arrays and connections.
- Add bindings for experimental `getDataID` function on the `Environment`. Won't 
document it for now because the Relay team suggests it's not stable, but it's needed 
to make Relay work with schemas that do not conform to the globally unique IDs 
requirement (Hasura GraphQL for instance).