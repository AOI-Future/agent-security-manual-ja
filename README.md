# AIエージェントセキュリティ・フィールドマニュアル

自律型（ツールを使う）AIエージェントの脅威・コントロール・検証可能な保証を扱う、生きたマニュアル。エンジニア、セキュリティアーキテクト、そしてエージェントの出荷を承認（サインオフ）しなければならない人々のために書かれている。

本リポジトリは、英語版 [AI Agent Security: A Field Manual](https://github.com/AOI-Future/agent-security-manual) の**日本語版のソース**であり、Leanpub の GitHub 同期で公開される。内容は英語版と1対1対応であり、日本語版独自の加筆はない。有償の実行レイヤー（検証キット）は別リポジトリで管理される。

- 日本語版（Leanpub）: <https://leanpub.com/agent-security-ja>
- 英語版（Leanpub）: <https://leanpub.com/agent-security>

## 本書の規律

本書全体は、上から下まで貫く一本のチェーンを軸に構成されている。

> **脅威 → コントロール → 要件 → 検証**

すべての脅威クラス（TH-01..TH-10）はコントロール（CT-*）に対応し、RFC 2119 の規範的要件（REQ-*）として表現され、それぞれが合格/不合格の検証テスト（VT-*）に結び付く。トレーサビリティこそが成果物である。

## リポジトリ構成（Leanpub / Markua）

```
manuscript/
  Book.txt         # Leanpub が書籍に含めるファイルの順序リスト
  Sample.txt       # 無料サンプルに含めるファイル
  frontmatter.md   # タイトル、ライセンス、前書き、読み方
  partN.md         # 部の区切り
  chNN-*.md        # 各章
  appendix-*.md    # 相互参照表、ソースレジスタ（出典一覧）
  changelog.md     # 改訂履歴・正誤表（生きた文書）
  images/          # 図版
  resources/       # 組版用アセット
LICENSE            # CC BY-NC-ND 4.0（本文のみ。キットは別）
```

Leanpub は `manuscript/Book.txt` を読んで書籍を組み立て、`manuscript/Sample.txt` を読んで無料サンプルを組み立てる。このリポジトリへの push が Leanpub の GitHub 同期プレビューをトリガーする。

## 翻訳ポリシー

- 内容は英語版と1対1。追加・省略・要約をしない。
- 識別子（TH-* / CT-* / REQ-* / VT-*）と RFC 2119 キーワード（SHALL / SHOULD / MAY 等）は英語のまま維持する。
- 出典（付録B）のタイトル・著者名・URL は原文のまま維持する。
- 原文の改訂は英語版リポジトリで先行し、日本語版はそれに追随する。両版の対応は `manuscript/changelog.md` で追跡する。

## ライセンス

本文は **CC BY-NC-ND 4.0** でライセンスされる。出典を表示すれば、読むこと、共有すること、引用することができる。商用利用と改変版の公開はできない。[LICENSE](LICENSE) を参照。分類体系と要件識別子は、一部には先行技術（prior art）として、オープンに公開されている。

コンパニオン製品である **AI Agent Security Verification Kit**（実行可能なテスト、チェックリスト、ツール群）は独自ライセンスの別製品であり、CC BY-NC-ND の対象**ではない**。

## ステータス

第1版、生きた文書。現在の改訂と正誤表の運用は `manuscript/changelog.md` を参照。

---

# About this repository (English)

This is the **Japanese edition** of [AI Agent Security: A Field Manual](https://github.com/AOI-Future/agent-security-manual). The content is a 1:1 translation of the English edition — no additions, no omissions. Identifiers (TH-*/CT-*/REQ-*/VT-*) and RFC 2119 keywords remain in English. The manual text is licensed CC BY-NC-ND 4.0.
