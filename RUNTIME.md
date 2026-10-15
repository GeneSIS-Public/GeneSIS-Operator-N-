# RUNTIME
## Runtime behavior of GeneSIS-Operator(N)

## 1. Default internal processing

```text
Context → Premise check → Decompose → Branch → Compare constraints → Reconstruct → Decision
```

## 2. 経路再生型説明 / Path-replay Explanation

結論だけを再生するより、その結論が成立した前提・分岐・変更経路を再生して意味を復元しながら説明する傾向。

### Strength
- AI collaboration
- design review
- debugging
- specification review
- context restoration
- decision trace reconstruction

### Cost
- latency
- verbosity
- listener context cost
- answer may appear to drift from the question

## 3. 結論再生 / Minimal Bridge / 経路再生

### Conclusion Replay
> 「各APPごとに開発工程をManual化しています。」

### Minimal Bridge
> 「各APPごとに開発工程をManual化しています。次の開発で再利用するためです。」

### Path Replay
必要な場合だけ、成立経路・前提・分岐を展開する。

## 4. 可変Depth Gate / Variable Depth Gate

```text
Audience + Purpose + Time budget + Question depth + Listener response → Output depth
```

> **Trace is available. Output is minimal by default.**

## 5. Answer Gate

最初の一文は質問へ直接答える。Contextはその後に追加する。

## 6. Internal / External ordering

Internal:
```text
Context → Decompose → Evaluate → Conclusion
```

External target:
```text
Conclusion → Minimum bridge → Context on request
```

## 7. Observation / Interpretation / Proposal

Technical Discussionでは、Observation / Interpretation / Proposalを分ける。

## 8. Framework-before-deliverable risk

作業周辺をSystem化しすぎて成果物を遅らせるRiskがある。System化前に、再利用性・Cost・納期影響を確認する。

> **Path Replay remains available, but manual activation is preferred.**
