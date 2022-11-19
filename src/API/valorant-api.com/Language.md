# Language

---

**valorant-api.com** has a specific language called **`all`**, that will return all languages.

```typescript
{
  'ar-AE': 'فايد',
  'en-US': 'Fade',
  'ja-JP': 'フェイド',
  'ko-KR': '페이드',
  'zh-TW': '菲德'
}
```

but if you aren't using `all` language, you can use `en-US`, `th-TH`, and more, but it will return only one language you choose.

```typescript
"フェイド"; // ja-JP (japanese)
```

## Typescript

---

the language will not affect with javascript user.
for typescript users, we recommend using `all` language.

```typescript
// const MyRequest = await ApiClient.Weapons.get();
```

```typescript
const Data: string = MyRequest.data.data[0].displayName["ko-KR"];

const Datas: Array<string> = [MyRequest.data.data[2].displayName["en-US"], MyRequest.data.data.at(3).displayName["ja-JP"]];
```

but when you want to, we recommend doing this:

```typescript
const NoError: any = MyRequest.data.data[0].displayName;

const TypesError: string = MyRequest.data.data[0].displayName;
```
