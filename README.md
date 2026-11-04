# skills

Yuta Kondo が作った Claude Code のスキルの一覧です。スキルの本体はそれぞれのリポジトリにあり、このリポジトリは「どこに何があるか」をまとめたカタログです。カタログを一度登録すれば、その中から欲しいスキルだけを選んで入れられます。

## 入れ方

カタログを登録します。

```text
/plugin marketplace add knk1313/skills
```

使いたいスキルを選んで入れます。`/plugin` の画面から選ぶこともできます。

```text
/plugin install paper-analysis@knk1313-skills
/plugin install docs-rules@knk1313-skills
/plugin install repo-kit@knk1313-skills
```

カタログに載ったスキルの更新を取り込むときは、次を実行します。

```text
/plugin marketplace update knk1313-skills
```

## スキルの一覧

### 調査系

| スキル | 内容 |
| --- | --- |
| [paper-analysis](https://github.com/knk1313/paper-analysis) | 論文1本を、本文に書かれた事実だけを根拠に読み解き、日本語のレポート（HTML）にまとめる。PDF、arXiv の URL や ID、DOI を渡して使う |

### 日常系

| スキル | 内容 |
| --- | --- |
| [docs-rules](https://github.com/knk1313/docs-rules) | 日本語の文書を、共通の表記・文体ルールと文書種別ごとの構成に沿って書く。セッションログ、提案書、論文、手順書、画面の文言などに使う |

### 開発系

| スキル | 内容 |
| --- | --- |
| [repo-kit](https://github.com/knk1313/repo-kit) | リポジトリの土台になるファイルを足す `setup` と、公開前の点検・検査・GitHub の設定を進める `publish` |

## スキルを足すとき

1. スキルのリポジトリのルートに `.claude-plugin/plugin.json` を置く
2. このリポジトリの `.claude-plugin/marketplace.json` の `plugins` に、そのリポジトリを指す1件を足す
3. この README の、当てはまる区分の表に1行足す

不具合や要望は、それぞれのスキルのリポジトリに Issue を立ててください。カタログそのものの誤り（リンク切れ、入れられないなど）は、このリポジトリに Issue を立ててください。

## ライセンス

[MIT](LICENSE)。各スキルのライセンスは、それぞれのリポジトリを参照してください。
