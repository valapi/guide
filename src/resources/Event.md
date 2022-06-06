# Event

-----------

```typescript
ApiClient.on('EVENT_NAME', callback());
```

- **ready** => `void`
- **request** => [`Request`](#request)
- **changeSettings** => `{ name:string, data:any }`
- **error** => [`Error`](#error)

## Request

```typescript
interface Error {
    method: string;
    url: string;
    body?: Object;
    config: AxiosRequestConfig;
}
```

## Error

```typescript
interface Error {
    errorCode: string;
    message: string;
    data: any;
}
```

# Example

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
}));
```