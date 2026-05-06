
## vscode markdown preview setting
目に優しい設定
VSCode で Cmd+Shift+P → "Markdown Preview Enhanced: Customize CSS" を実行し設定用のcssファイルを開く。

https://shd101wyy.github.io/markdown-preview-enhanced/#/customize-css

```css
/* Please visit the URL below for more information: */
/*   https://shd101wyy.github.io/markdown-preview-enhanced/#/customize-css */

.markdown-preview.markdown-preview {

  // ── Layout ──────────────────────────────────────────────────────────
  padding: 1rem 2rem;

  // ── Base Typography ─────────────────────────────────────────────────
  font-size: 17px;
  // 1.75: WCAG recommends ≥1.5; slightly higher for dark bg comfort
  line-height: 1.75;
  // #d4d4d4 on #24292e = ~9.2:1 contrast ratio, exceeds WCAG AAA (7:1)
  color: #d4d4d4;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Noto Sans', sans-serif;
  word-spacing: 0.02em;

  // ── Paragraphs ──────────────────────────────────────────────────────
  p {
    margin-top: 0;
    margin-bottom: 1.25em;
  }

  // ── Headings ────────────────────────────────────────────────────────
  h1, h2, h3, h4, h5, h6 {
    line-height: 1.3;
    margin-top: 2em;
    margin-bottom: 0.6em;
    color: #f0f0f0;
  }
  h1 {
    font-size: 2em;
    background-color: #1d5494;
    padding: 0.35em 0.6em;
    border-radius: 6px;
    border-bottom: none;
  }
  h2 {
    font-size: 1.6em;
    background-color: #174280;
    padding: 0.25em 0.6em;
    border-radius: 4px;
    border-bottom: none;
  }
  h3 { font-size: 1.3em; }
  h4 { font-size: 1.1em; }

  // ── Code ────────────────────────────────────────────────────────────
  code {
    font-family: 'SFMono-Regular', Consolas, 'Liberation Mono', Menlo, monospace;
    font-size: 0.88em;
    background-color: #2d333b;
    padding: 0.15em 0.45em;
    border-radius: 4px;
  }
  pre {
    background-color: #1e2228;
    border: 1px solid #373e47;
    border-radius: 6px;
    padding: 1.2em 1.5em;
    line-height: 1.6;
    overflow-x: auto;

    code {
      background: none;
      padding: 0;
      font-size: 0.87em;
    }
  }

  // ── Blockquote ──────────────────────────────────────────────────────
  blockquote {
    border-left: 4px solid #4a8eda;
    padding: 0.5em 1em;
    margin: 1.5em 0;
    color: #a8b2c0;
    background-color: #2a2f37;
    border-radius: 0 4px 4px 0;
  }

  // ── Links ───────────────────────────────────────────────────────────
  a {
    color: #58a6ff;
    text-decoration: none;
    &:hover { text-decoration: underline; }
  }

  // ── Lists ───────────────────────────────────────────────────────────
  ul, ol {
    padding-left: 1.8em;
    margin-bottom: 1em;

    li {
      margin-bottom: 0.4em;
      line-height: 1.7;
    }
  }

  // ── Tables ──────────────────────────────────────────────────────────
  table {
    th {
      background-color: #2d333b;
      color: #f0f0f0;
      padding: 10px 16px;
    }
    td {
      padding: 8px 16px;
    }
    tr:nth-child(even) { background-color: #272c32; }
  }

  // ── Horizontal Rule ─────────────────────────────────────────────────
  hr {
    border: none;
    border-top: 1px solid #404040;
    margin: 2.5em 0;
  }
}
```