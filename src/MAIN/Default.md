# Default Import

Default imports are recommended for javascript

because javascript cannot use type definition then we can only use client

-----------

## Import

```javascript
const { Auth, WebClient, RiotAPI, ValorantApiCom } = require('valorant.ts').default
```

## Usage

Packages

```javascript
const AuthClient = new Auth( config? );
```

API

```javascript
const ApiClient = new WebClient( config? );
```

```javascript
const ApiClient = new RiotAPI( config? );
```

```javascript
const ApiClient = new ValorantApiCom( config? );
```