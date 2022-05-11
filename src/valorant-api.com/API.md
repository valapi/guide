# API

-----------

All API Base On [dash.valorant-api.com](https://dash.valorant-api.com/)

*( comming soon... )*

<details>
<summary>Example</summary>
<blockquote>

```typescript
//Returns data and assets of all weapon buddies
await ApiClient.Buddies.get();

//Returns data and assets of all weapon buddy levels
await ApiClient.Buddies.getLevels();

//Returns data and assets of the requested weapon buddy
await ApiClient.Buddies.getByUuid('uuid');

//Use the isPlayableCharacter=true filter to make sure you don't have a "duplicate" Sova.
await ApiClient.Agents.get(true);
```

</blockquote>
</details>

## Usage

```typescript
const _data = await ApiClient.{Endpoints}.{Function}
```