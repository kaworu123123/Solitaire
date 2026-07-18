# Solitaire（開発用配布）

SolitaireClassic の **開発 APK** と **アップデート情報** を GitHub Releases に集約します。

## 構成

| もの | 場所 |
|------|------|
| 版情報 `app_version.json` | このリポの `main` |
| APK | [Releases](https://github.com/kaworu123123/Solitaire/releases) のアセット `SolitaireClassic.apk` |
| 版情報（Release にも添付） | 各 Release の `app_version.json` |

## アプリ側の参照

- JSON: `https://raw.githubusercontent.com/kaworu123123/Solitaire/main/app_version.json`
- 最新 Release API: `https://api.github.com/repos/kaworu123123/Solitaire/releases/latest`

## 公開手順（Unity）

1. `Tools → Solitaire → Dev Update → Set Solitaire Repo Folder...`（例: `E:\dev\Solitaire`）
2. `Tools → Solitaire → Dev Update → Set GitHub Token...`（`repo` 権限の PAT）
3. Android ビルド（自動で版上げ → JSON push → Release 作成 → APK アップロード）

手動で APK だけ上げる場合: `Tools → Solitaire → Dev Update → Publish APK to GitHub Release...`
