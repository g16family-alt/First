
# 📅 Instagram投稿カレンダー自動生成（API不要・Streamlit）

スマホ・PC両対応。ボタン1つで**今日から30日分**の計画＋**新ネタ10本**を自動追加し、チェックリスト付きExcelをダウンロードできます。

## 使い方（Streamlit Community Cloud公開）
1. このリポジトリをGitHubにアップロード（`streamlit_app.py`, `requirements.txt` を含める）
2. https://share.streamlit.io/ にアクセスしてGitHubを連携
3. 「New app」→ リポジトリ／ブランチ／ファイルとして `streamlit_app.py` を指定 → Deploy
4. 発行されたURLをスマホで開いて利用（ブックマーク推奨）

## ローカル実行
```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
```

## 主な機能
- 基本テンプレート（最大60本まで指定可能、初期値30本）
- **新ネタ自動追加（最大30本）**：100本の事前リストから毎回ランダム、重複回避ロジック付き
- 進捗管理カラム（撮影完了／編集完了／投稿完了／メモ）
- Excelダウンロード（`Instagram_Post_Calendar_Auto.xlsx`）
