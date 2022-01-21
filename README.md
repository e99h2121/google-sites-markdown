# Google Sites Markdown

As Google Sites doesn't support Tables or Markdown, this script allows you to write Markdown inside a HTML snippet within Google Sites.

Google SitesはテーブルやMarkdownをサポートしていない。このスクリプトを使えば、Google Sites内のHTMLスニペットの中にMarkdownを記述することができる。

## Usage

1. While editing a Google Site page double click to bring up the page options
2. Select `<> Embed`
3. Change to the `Embed Code` tab
4. Paste the code below from the example and replace Markdown with your own
5. Save

## Code snippets

If you wish to use code snippets inside your markdown, you'll need to escape the backticks:

```typescript
\`\`\`typescript
function getBestHero(spiderman: string): boolean {
  return true
}

const isSpidermanTheBestHero = getBestHero('spiderman')
\`\`\`
```

## Example

```html
<script src="https://cdn.jsdelivr.net/gh/e99h2121/google-sites-markdown/index.js"></script>

<script>
markdown`

# マークダウン

マークダウンでGoogle Sitesを書けます

> テーブルも？

- [X] はい
- [ ] いいえ

## 表

| ID  | Name         | Hero      |
| --- | ------------ | --------- |
| 1   | Peter Parker | Spiderman | 
| 2   | Bruce Wayne  | Batman    |

*リストは*

- もちろん
- Hooray! 🎉
`
</script> 
```
