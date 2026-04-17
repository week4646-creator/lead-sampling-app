# 鉛塗料サンプリング PWA

EPA RRP / HUD 準拠の鉛塗料（ペイントチップ）フィールドサンプリング PWA。
アスベストバルクサンプリングアプリ（`bulk-sampling-app`）を流用して作成。

## 特徴

- 単一HTMLファイル（React 18 CDN、ビルド不要）
- PWA インストール対応（オフライン動作）
- サンプル番号・写真・図面マッピング・場所情報を現場で記録
- CSV / Excel / フォトログ(DOCX) / アセスメントシート / 写真ZIP の出力
- CSV / COC / 写真ZIP のインポート
- 表示項目のユーザー設定（デフォルト8項目、追加で9項目を任意表示）
- ダークモード・シンプルモード

## 使い方

1. `lead-sampling.html` をブラウザで開く（またはGitHub Pagesから）
2. シンプル/フルモードを選択
3. プロジェクト情報を入力
4. サンプル追加 → 写真撮影・情報入力 → 図面にピン配置
5. サイドバーからエクスポート

## データ永続化

- **localStorage** (`lead-paint-sampling-projects`): プロジェクト一覧
- **IndexedDB** (`lead-paint-photos`): 写真・図面実データ
- PWA install 推奨（iPhone Safari / Android Chrome で最も安定）

## ドメイン項目（鉛塗料サンプリング）

- 塗装部位（Door/Window/Wall など 32種類）
- 下地材（Wood/Metal/Drywall など 10種類）
- 塗膜状態（Intact / Fair / Poor — HUD基準）
- 塗膜層数（Single / Multi-Layer 2-3 / 4+ / Unknown）
- 色 14種類（White / Yellow / Red / Pink / ...）

## ライセンス

Private.
