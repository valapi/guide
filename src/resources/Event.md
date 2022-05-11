# Event

-----------

```typescript
ApiClient.on('EVENT_NAME', callback()) 
```

- **ready**
- **changeSettings** => `{ name:string, data:any }`
- **error** => `Error`

## Error

-----------

```typescript
interface Error {
    errorCode: string,
    message: string,
    data: any,
}
```

## Example

-----------

*Ready*

```typescript
ApiClient.on('ready', (() => {
    console.log('Client is ready!');
}));
```

*changeSettings*

```typescript
ApiClient.on('changeSettings', ((data: { name:string, data:any }) => {
    console.log(data);
}));
```

*Error*

```typescript
ApiClient.on('error', ((data: Error) => {
    console.log(data);
}))
```