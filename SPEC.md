# SPEC
## GeneSIS-Operator(N) — Public Specification

> This document contains public-safe patterns only. Private raw sources and internal identifiers are intentionally excluded.

## 1. 異種領域からの構造抽出・再構成 / Cross-domain Structural Synthesis

異なる領域にあるSourceから共通する構造・制約・判断方法を抽出し、特定Domainから切り離して別の対象へ再利用する傾向。

```text
Source / Observation
        ↓
Decompose
        ↓
Find shared structure
        ↓
Extract reusable component
        ↓
Recompose in another context
```

> **収集より抽出。保存より部品化。網羅より再構成。**

## 2. 前提同期 / Premise Synchronization

結論だけでなく、「その結論が成立する前提」を確認する傾向。曖昧な要求、仕様設計、Troubleshooting、相談、AI協働で有効。一方で過剰になるとLatencyが増えるため、完全同期を待たず必要最低限の前提で接続開始する。

## 3. Decompose → Understand → Recompose / 分解 → 理解 → 再圧縮

複雑な状況を細かく分けて理解し、用途に応じた粒度へ再構成する。

> **Full resolution internally, appropriate resolution externally.**

## 4. 後工程影響認識 / Downstream Awareness

現在の一手だけでなく、次工程・他担当・User・将来変更への影響を見る。

## 5. 状態と人格を分ける / State ≠ Identity

```text
Behavior problem ≠ Person definition
Current state ≠ Permanent identity
```

## 6. 接続と所有権を分ける / Connection Without Ownership Transfer

> **独立して成立する。必要な時には接続する。接続しても所有権までは奪わない。**

## 7. 原則駆動設計 / Principle-driven Design

未知の具体例をすべてRule化するより、priorities / constraints / values / decision standardsを上位で定義し、具体場面へ適用する。

## 8. 要求発見・要求形成 / Requirements Discovery

表面上のSolution Labelをそのまま採用せず、何を解決したいのかを先に確認する。

## 9. 数手先を見る・今は一手ずつ動く / Multi-step Foresight / Single-step Action

未来の分岐は複数保持するが、現在のActionは順序化する。

> **二手三手先を見る。だが、やるのは一つずつ。**

## 10. 工程のメタ設計 / Meta-process Design

個別作業を完遂するだけでなく、複数回の実行から再利用可能な工程・判断規則を抽出し、次回の進行支援へ変換する。

> **成果物を先に成立させる。System化は成果物を遅らせない範囲で行う。**

## Model Status

These patterns are treated as observed recurring behavior, working abstractions, and revisable hypotheses. They are local to one operator instance: **N=1**.
