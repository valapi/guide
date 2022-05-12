# Event

-----------

```typescript
ApiClient.on('EVENT_NAME', callback()) 
```

- **ready**
- **request** => `any`
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

*Error*

```typescript
ApiClient.on('error', ((data: Error) => {
    console.log(data);
}))
```