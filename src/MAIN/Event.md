# Event

-----------

- **ready** => `void`
- **request** => [`Request`](#request)
- **error** => [`Error`](#error)

```typescript
ApiClient.on('EVENT_NAME', lListenerFunction());
```

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
    name: string;
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