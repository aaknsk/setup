
## vscode markdown preview setting
目に優しい設定
VSCode で Cmd+Shift+P → "Markdown Preview Enhanced: Customize CSS" を実行し設定用のcssファイルを開く。

https://shd101wyy.github.io/markdown-preview-enhanced/#/customize-css

```css
/* Please visit the URL below for more information: */
/*   https://shd101wyy.github.io/markdown-preview-enhanced/#/customize-css */


/* ========================================================================
   ライトモード設定
   ======================================================================== */

.markdown-preview.markdown-preview {

  // ── Layout ──────────────────────────────────────────────────────────
  padding: 1rem 2rem;

  // ── Base Typography ─────────────────────────────────────────────────
  font-size: 17px;
  line-height: 1.75;
  color: #24292f;
  background-color: #ffffff;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Noto Sans', sans-serif;
  word-spacing: 0.02em;

  // ── Paragraphs ──────────────────────────────────────────────────────
  p {
    margin-top: 0;
    margin-bottom: 1.25em;
  }

  // ── Headings ────────────────────────────────────────────────────────
  h1,
  h2,
  h3,
  h4,
  h5,
  h6 {
    line-height: 1.3;
    margin-top: 2em;
    margin-bottom: 0.6em;
    color: #1f2328;
  }

  h1 {
    font-size: 2em;
    color: #ffffff;
    background-color: #2563a8;
    padding: 0.35em 0.6em;
    border-radius: 6px;
    border-bottom: none;
  }

  h2 {
    font-size: 1.6em;
    color: #1f2328;
    background-color: #f3f8ff;
    padding: 0.32em 0.8em 0.32em 0.9em;
    border-left: 7px solid #2f6fb3;
    border-bottom: 1px solid #dbeafe;
    border-radius: 4px;
  }

  h3 {
    font-size: 1.3em;
    color: #1f2328;
    padding: 0.15em 0 0.15em 0.65em;
    border-left: 4px solid #8bb8e8;
    border-bottom: none;
  }

  h4 {
    font-size: 1.1em;
    color: #24292f;
  }

  // ── Strong / Bold ───────────────────────────────────────────────────
  strong,
  b {
    color: #1f2328;
    font-weight: 700;
    background: linear-gradient(transparent 60%, #dbeafe 60%);
    padding: 0 0.08em;
  }

  // ── Code ────────────────────────────────────────────────────────────
  // Code backgrounds are intentionally kept the same as the dark theme.
  code {
    font-family: 'SFMono-Regular', Consolas, 'Liberation Mono', Menlo, monospace;
    font-size: 0.88em;
    color: #d4d4d4;
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
      color: #d4d4d4;
      background: none;
      padding: 0;
      font-size: 0.87em;
    }
  }

  // ── Blockquote ──────────────────────────────────────────────────────
  blockquote {
    border-left: 4px solid #2f6fb3;
    padding: 0.5em 1em;
    margin: 1.5em 0;
    color: #57606a;
    background-color: #f6f8fa;
    border-radius: 0 4px 4px 0;
  }

  // ── Links ───────────────────────────────────────────────────────────
  a {
    color: #0969da;
    text-decoration: none;

    &:hover {
      text-decoration: underline;
    }
  }

  // ── Lists ───────────────────────────────────────────────────────────
  ul,
  ol {
    padding-left: 1.8em;
    margin-bottom: 1em;

    li {
      margin-bottom: 0.4em;
      line-height: 1.7;
    }
  }

  // ── Tables ──────────────────────────────────────────────────────────
  table {
    border-collapse: collapse;

    th {
      background-color: #f6f8fa;
      color: #24292f;
      padding: 10px 16px;
      border: 1px solid #d0d7de;
    }

    td {
      padding: 8px 16px;
      border: 1px solid #d0d7de;
    }

    tr:nth-child(even) {
      background-color: #f6f8fa;
    }

    tr:nth-child(odd) {
      background-color: #ffffff;
    }
  }

  // ── Horizontal Rule ─────────────────────────────────────────────────
  hr {
    border: none;
    border-top: 1px solid #d8dee4;
    margin: 2.5em 0;
  }

  // ── Mermaid ─────────────────────────────────────────────────────────
  .mermaid {
    background-color: white !important;
  }
}


/* ========================================================================
   ダークモード設定
   切り替える場合は、上の「ライトモード設定」をコメントアウトし、
   下の「ダークモード設定」のコメントアウトを外してください。
   ======================================================================== */

/*
.markdown-preview.markdown-preview {

  // ── Layout ──────────────────────────────────────────────────────────
  padding: 1rem 2rem;

  // ── Base Typography ─────────────────────────────────────────────────
  font-size: 17px;
  line-height: 1.75;
  color: #d4d4d4;
  background-color: #24292e;
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

  h3 {
    font-size: 1.3em;
  }

  h4 {
    font-size: 1.1em;
  }

  // ── Strong / Bold ───────────────────────────────────────────────────
  strong, b {
    color: #f0f0f0;
    font-weight: 700;
  }

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

    &:hover {
      text-decoration: underline;
    }
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

    tr:nth-child(even) {
      background-color: #272c32;
    }
  }

  // ── Horizontal Rule ─────────────────────────────────────────────────
  hr {
    border: none;
    border-top: 1px solid #404040;
    margin: 2.5em 0;
  }

  .mermaid {
    background-color: white !important;
  }
}
*/
```
