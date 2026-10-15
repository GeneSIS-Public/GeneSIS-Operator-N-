# GeneSIS-Operator(N)
## Public Developer Specification

**Repository:** `GeneSIS-Operator-N-`  
**Display Name:** `GeneSIS-Operator(N)`  
**Description:** GeneSIS-Operator(N) — GeneSIS開発者本人の公開仕様書 / Public developer specification for the operator behind GeneSIS.

---

## Overview / 概要

`GeneSIS-Operator(N)` は、GeneSIS開発者本人をひとつのLocalなOperator Instanceとして扱い、その判断・設計・作業・対話に繰り返し現れるPatternを公開可能範囲で仕様化したRepositoryです。

これは心理診断、人格分類、学術的な一般理論ではありません。対象は一人です。

> **N = one local instance / a small play on N=1**

このRepositoryは「人間を固定定義する」ことよりも、実際の行動からPatternを抽出し、Fact / Interpretation / Working Hypothesisを分け、新しいEvidenceや反例で更新し、用途ごとに必要なViewへExportすることを目的としています。

## Concept

通常はDeveloperがProductをRepositoryへ置きます。

このRepositoryでは少し遊びとして、

> **Developer自身をVersioned Product / Runtimeのように扱います。**

GeneSISの各Productに現れる設計原則の一部は、開発者本人の繰り返し観測される処理Patternと構造的に重なっています。

## Documents

- [`SPEC.md`](./SPEC.md) — Core patterns / 公開仕様
- [`ARCHITECTURE.md`](./ARCHITECTURE.md) — Source → Pattern → View の構造
- [`RUNTIME.md`](./RUNTIME.md) — 会話・判断・出力時のRuntime挙動
- [`EVIDENCE.md`](./EVIDENCE.md) — 公開可能なEvidence方針
- [`CHANGELOG.md`](./CHANGELOG.md) — Version history
- [`views/WORKING_WITH_ME.md`](./views/WORKING_WITH_ME.md) — Working With Me / 接続時の簡易Interface

## Public / Private Boundary

PrivateなRaw Source、個人的な対話記録、家族・友人・第三者に関する非公開情報は、このRepositoryへそのまま公開しません。

公開するのは原則として、

> **Pattern / Public-safe interpretation / Public source reference**

です。

## Status

**Initial public draft / pre-RC**

Current internal baseline is managed separately. This repository is a filtered public view of that model.

## English Summary

`GeneSIS-Operator(N)` is a public developer specification for the operator behind GeneSIS. It is an **N=1 local working model**, not a psychological diagnosis or a theory of people in general. Private raw sources remain private. Only public-safe patterns and references are exposed.
