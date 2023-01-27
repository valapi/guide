# Event

---

-   **request** => [`Request`](#request)
-   **error** => [`Error`](#error)

```typescript
ApiClient.on("EVENT_NAME", lListenerFunction());
```

## Request

```typescript
interface Error {
    method: string;
    url: string;
    body: any;
    config: AxiosRequestConfig;
}
```

## Error

```typescript
interface Error {
    name: string;
    message: string;
    stack?: string;
    data: any;
}
```

# Example

---

_Error_

```typescript
ApiClient.on("error", (data: Error) => {
    console.log(data);
});
```
