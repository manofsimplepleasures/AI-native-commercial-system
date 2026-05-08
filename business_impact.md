# Business Impact Framework

Use this document to evaluate commercial value, not just prompt quality.

## 1. Core metrics

### 1) signal_to_outreach_rate

```text
approved_outreach_items / detected_high_relevance_signals
```

Interpretation:
- low value means filtering is too strict or process is blocked,
- very high value may indicate weak qualification discipline.

### 2) reply_rate

```text
replies / first_touch_messages_sent
```

Interpretation:
- indicates angle relevance and timing quality,
- compare by channel and segment.

### 3) meeting_rate

```text
qualified_calls / first_touch_messages_sent
```

Interpretation:
- stronger indicator than reply_rate for BizDev quality.

### 4) proposal_discussion_rate

```text
proposals_discussed_live / proposals_sent
```

Interpretation:
- direct signal of process discipline,
- low value = "proposal in void" anti-pattern.

### 5) win_rate

```text
closed_won / qualified_opportunities
```

Interpretation:
- quality of qualification + offer match + follow-up execution.

### 6) cycle_days

```text
decision_date - signal_detected_date
```

Interpretation:
- tracks speed and operational friction.

## 2. Quality metrics

- `anti_generic_pass_rate`: % outputs passing QA on first run,
- `human_rewrite_rate`: % outputs requiring major manual rewrite,
- `false_positive_signal_rate`: % qualified leads later marked irrelevant.

## 3. Business review cadence

- weekly: review activity and process metrics,
- bi-weekly: review conversion and stage leakage,
- monthly: update prompts, routing rules, and offer ladder assumptions.

## 4. Decision rules

- if reply rate is stable but meeting rate drops -> revise CTA and qualification logic,
- if meeting rate is stable but win rate drops -> revise product match and proposal structure,
- if cycle expands >20% for 2 consecutive periods -> audit follow-up and handoff points.
