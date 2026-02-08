---
name: ios-app-e2e
description: End-to-end workflow for building and shipping a small iOS app from planning through App Store release. Use when Codex needs to run repeatable iOS delivery steps such as MVP definition, Xcode project setup, SwiftUI/MVVM implementation, testing, TestFlight distribution, and App Store submission.
---

# iOS App E2E

## Overview

Execute a repeatable workflow to deliver a small iOS app from idea to App Store submission in 14 days.

## Workflow

1. Define MVP scope in three features or fewer.
2. Implement in short daily slices with a running build.
3. Extract reusable steps after each day.
4. Ship to TestFlight before App Store submission.

## Step 1: Define Scope

- Write one-sentence product goal.
- Fix MVP to three user-facing capabilities.
- Define success criteria with concrete dates.

## Step 2: Setup Project

- Create Xcode project with SwiftUI + MVVM.
- Establish branch and PR workflow.
- Add minimum app metadata and bundle configuration.

## Step 3: Implement Core Features

- Build data model and persistence.
- Build list and create/delete flows.
- Build daily completion and streak calculation.
- Keep features behind simple, testable ViewModels.

## Step 4: Stabilize Quality

- Add unit tests for streak and persistence behavior.
- Run manual checks on at least one simulator and one device when available.
- Resolve crash and data-loss risks before polish work.

## Step 5: Ship

- Prepare icon, screenshots, description, and privacy details.
- Archive and distribute via TestFlight.
- Resolve tester feedback and submit to App Store.

## References

- Use `references/workflow-checklist.md` for daily shipping checklist.
- Use `references/release-readiness.md` for release gate criteria.
