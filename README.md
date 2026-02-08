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
