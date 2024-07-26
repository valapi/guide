# Language

---

**valorant-api.com** has a specific language called **`all`**, that will return all languages.

Example:

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

Example:

```typescript
"フェイド"; // ja-JP (japanese)
```
