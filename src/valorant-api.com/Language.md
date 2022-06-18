# Language

-----------

**valorant-api.com** have specific language call **`all`**, that will return all languages.

```typescript
{
  'ar-AE': 'فايد',
  'en-US': 'Fade',
  'ja-JP': 'フェイド',
  'ko-KR': '페이드',
  'zh-TW': '菲德'
}
```

but if you aren't use `all` language, you can use `en-US`, `th-TH` and more, but it will return only one language you choose.

```typescript
'フェイド' // ja-JP (japanese)
```

## Typescript

-----------

language will not affect with javascript user.
for typescript user we recommend to use `all` language.

```typescript
// const MyRequest = await ApiClient.Weapons.get();
```

```typescript
const Data: string = MyRequest.data.data[0].displayName['ko-KR']

const Datas: Array<string> = [

    MyRequest.data.data[2].displayName['en-US'],
    MyRequest.data.data.at(3).displayName['ja-JP'],

];
```

but when you use other language, we recommend to do this:

```typescript
const NotError: any = MyRequest.data.data[0].displayName;

const TypesError: string = MyRequest.data.data[0].displayName;
```