# portal-site2025 CLAUDE.md

## プロジェクト概要
教員向けの授業資料管理ポータル。
各授業のPDF資料（スライド・ハンドアウト）とHTMLページを一元管理する。

## 対象ユーザー
教員のみ（学生向け公開サイトではない）

## ディレクトリ構成
```
portal-site2025/
├── CLAUDE.md
├── index.html                     # 全授業の一覧ページ
├── probability2025/               # 確率（2025年度）
│   ├── index.html
│   ├── first01.pdf ~ first14.pdf
│   ├── second01.pdf ~ second12.pdf
│   └── handout_kakuritsu.pdf
└── information_literacy2025/      # 情報リテラシー（2025年度）
    ├── index.html
    ├── slide_first01-14.pdf
    ├── slide_second01-14.pdf
    ├── handout_first01-14.pdf
    └── handout_second01-14.pdf
```

## ファイル命名規則
- スライド: `slide_{first|second}{連番2桁}.pdf`
- ハンドアウト: `handout_{first|second}{連番2桁}.pdf`
- 授業フォルダ名: `{授業名}{年度}/`（例: `probability2025/`）

## 新授業を追加するときのルール
1. `{授業名}{年度}/` フォルダを作成する
2. PDFを命名規則に従って配置する
3. `index.html` を既存授業を参考に作成する
4. トップの `index.html` に授業リンクを追加する
5. この `CLAUDE.md` のディレクトリ構成を更新する

## Claudeへの指示
- ファイル構成を変更する場合は必ずこのCLAUDE.mdも更新すること
- 命名規則から外れたファイルがあれば指摘すること
- 新年度対応（2025→2026）の際は年度の一括置換を行うこと
