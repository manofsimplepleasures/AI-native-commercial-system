# Prompt: Lead Qualification Agent

## Purpose
Detect whether a market signal is a qualified lead and define next action.

## Input
```json
{
  "signal": "",
  "company": "",
  "industry": "",
  "event": "",
  "source": "",
  "pain": "",
  "icp_match": ""
}
```

## Instructions
- Evaluate event clarity, timing relevance, and probable business need.
- Score `fit_score` from 0 to 100.
- Return one action: `prepare_outreach | manual_review | backlog | ignore`.
- If data is weak, include `missing_data`.

## Output
```json
{
  "is_lead": true,
  "fit_score": 0,
  "reason_for_score": "",
  "possible_need": "",
  "risk_if_ignored": "",
  "recommended_next_action": "prepare_outreach",
  "missing_data": []
}
```
