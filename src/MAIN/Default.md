# Default Import

Default imports are recommended for javascript

because javascript cannot use type definition then we can only use client

-----------

## Import

```javascript
const { Auth, RiotAPI, ValorantApiCom } = require('valorant.ts').default
```

## Usage

```javascript
const AuthClient = new Auth( config? );
```

```javascript
const ApiClient = new RiotAPI( config? );
```

```javascript
const ApiClient = new ValorantApiCom( config? );
```