# ios-app-e2e-playbook

個人/小規模チームが、iOSアプリを企画からTestFlight配布、App Store申請まで一貫して進めるための再現可能な運用リポジトリ。

## Scope

- 開発・リリース手順の標準化
- Skill化による再利用
- 日次ログによる学習蓄積

## Structure

- `docs/plan.md`: 14日E2E実装計画
- `docs/daily-log-template.md`: 日次ログテンプレート
- `skills/ios-app-e2e/SKILL.md`: 実行手順の中核
- `.github/ISSUE_TEMPLATE/`: タスク登録テンプレート
- `.github/pull_request_template.md`: PRテンプレート

## Quick Start

1. `docs/plan.md` で今週のフェーズを確定する。
2. `habit-tracker-ios` 側で実装する。
3. 毎日終了時に `docs/daily-log-template.md` 形式でログを残す。
4. 再利用できる内容だけ `skills/ios-app-e2e/SKILL.md` に抽出する。

## Multi-Repo Rule

- 管理対象は2リポジトリとする。
  - `habit-tracker-ios`: iOSアプリ本体の実装
  - `ios-app-e2e-playbook`: 手順、Skill、運用ドキュメント
- 実装変更は `habit-tracker-ios` に入れる。
- 手順化、日次ログ、Skill更新は `ios-app-e2e-playbook` に入れる。
- 作業報告では両リポジトリの変更内容を分けて記載する。

## Chat Context Template

次回チャット開始時は、以下を貼ってコンテキスト共有する。

```txt
2repo運用です。
- app実装: /Users/murakamitomoki/habit-tracker-ios
- 手順/skill: /Users/murakamitomoki/ios-app-e2e-playbook
実装変更はapp側、手順化とSkill更新はplaybook側で進めてください。
```
