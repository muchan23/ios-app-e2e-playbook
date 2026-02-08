# Archive / 署名 / バージョン運用

## 1. ビルド前準備

- `Version` と `Build` を更新する。
- Release構成で警告・エラーがないことを確認する。
- Bundle IdentifierとTeam設定を確認する。

## 2. 署名設定

- `Signing & Capabilities` で Release が自動署名または意図した手動署名になっている。
- プロビジョニングプロファイルが有効期限内である。

## 3. Archive

- Xcodeで `Any iOS Device` を選択する。
- `Product > Archive` を実行する。
- Organizerでアーカイブを選択し、`Distribute App` から `App Store Connect` を選ぶ。

## 4. アップロード後

- App Store Connectで該当ビルドが処理完了になるまで待つ。
- 処理完了後に対象バージョンへビルドを紐づける。

## 運用ルール

- 同じ提出単位でBuild番号は単調増加させる。
- 審査差し戻し修正版はVersionを維持し、Buildのみ増やす。
