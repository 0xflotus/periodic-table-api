# periodic-table-api
A Node.js API to access the Periodic Table elements in JSON format. Hosted on Firebase.

## Elements
Each element has the same structure:

```
{
  atomicNumber: number,
  symbol: string,
  name: string,
  mass: number,
  electronConfiguration: string,
  group: string
}
```

## How it works
There are several ways to fetch elements from the periodic table:

### All
- https://ptab-api.web.app/

This will fetch all the 118 elements at once.

### By group
- https://ptab-api.web.app/group?g=actinide

This will fetch all the elements that belong to the actinide group. You can change "actinide" for the group you want to access.

### Individually
- https://ptab-api.web.app/element?atomicNumber=94 or https://ptab-api.web.app/element?z=94

This will fetch the element with atomic number (Z) 94. You can change "94" for the atomic number of the element you want to access.

- https://ptab-api.web.app/element?symbol=pu

This will fetch the element with symbol Pu. You can change "pu" for the symbol of the element you want to access.

- https://ptab-api.web.app/element?name=plutonium

This will fetch the element with name Plutonium. You can change "plutonium" for the name of the element you want to access.

**NOTE:** both the search by symbol and name are not case-sensitive.
