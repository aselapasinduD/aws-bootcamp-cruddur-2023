# Week 0 — Billing and Architecture

## Create an AWS Budget

Get your AWS Account ID\
```aws sts get-caller-identity --query Account --output text```

Create Budget\
```aws budgets createl-budget \
    --accountl-id=AccountID \
    --budget=file://aws/json/budget.json \
    --notifications-with-subscribers-file://aws/json/budget-notifications-with-subscribers.json```