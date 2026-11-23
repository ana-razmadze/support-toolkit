# Sample Support Report

This report uses **made-up data** from a pretend shop, BrightCart: 80 tickets in [sample-tickets.csv](sample-tickets.csv). I made the data a bit messy on purpose, so there is something to find and fix.

The goal is to show how I read numbers and turn them into actions.

## Main numbers

| Metric | Result |
|---|---|
| Tickets | 80 |
| Solved within 24 hours | 67.5% |
| Median time to solve | 10.7 hours |
| Escalated tickets | 7 (8.8%) |
| Average CSAT (1–5) | 4.01 |

The goal for "solved within 24 hours" is 95%. We are far from it.

## First reply time by channel

| Channel | Tickets | Median first reply |
|---|---|---|
| Phone | 15 | 1 minute |
| Chat | 30 | 6 minutes |
| Email | 35 | 104 minutes |

Email is the biggest channel (44% of tickets) and the slowest.

## By problem type

| Category | Tickets | Average hours to solve | Solved in 24h |
|---|---|---|---|
| Refund | 18 | 24.4 | 56% |
| Login problem | 7 | 19.0 | 57% |
| Payment issue | 16 | 16.9 | 69% |
| Wrong item | 8 | 15.8 | 75% |
| Order delay | 27 | 15.2 | 70% |
| Other | 4 | 12.4 | 100% |

## What I see

1. **Refunds are the slowest.** They take about 24 hours on average, and only 56% are done in a day.
2. **Order delays are the biggest group** (27 of 80 tickets, about one third). Customers are asking "where is my order?"
3. **Escalated tickets make customers unhappy.** CSAT is 3.0 for escalated tickets and 4.11 for the others. The wait hurts more than the problem.
4. **Email first replies are slow** (median 104 minutes).

## What I would do

| Problem | Action | How I would measure it |
|---|---|---|
| Too many "where is my order?" tickets | Add a tracking link to the shipping email. Publish the [article](../knowledge-base/where-is-my-order.md) | Order delay tickets go down 30% in a month |
| Slow refunds | Let L1 approve refunds under a set amount, with no manager step | Refunds solved in 24h from 56% to 85% |
| Escalated customers unhappy | Send an update every 4 hours while the ticket waits, using [template 6](../reply-templates/templates.md) | Escalated CSAT from 3.0 to 3.8 |
| Slow email replies | Send an auto reply with the key articles, and check email every 2 hours | Median first reply under 60 minutes |
| Login tickets repeat | Make the reset-password link easier to find | Login tickets go down 40% |

## How the report was made

The data was generated with a small script using a fixed random seed, then calculated with Python. The numbers above come directly from the CSV file, so anyone can open the file and check them.

*In a real job I would use real ticket exports from tools like Zendesk or Help Scout, and update this report every week.*
