# Contractor chart of accounts (CSV)

A contractor's chart of accounts should put job costs on the same lines as the
estimate (direct labor, materials, subcontractors, equipment, permits), so the
profit and loss reads against the bid. It also needs retainage on both sides
(receivable from customers, payable to subs) and two month-end lines for
progress billing that runs ahead of or behind the work: costs and estimated
earnings in excess of billings (underbilled, an asset) and billings in excess
of costs and estimated earnings (overbilled, a liability). ZeraBooks' guide to
[bookkeeping for contractors](https://www.zerabooks.com/bookkeeping-for-contractors)
shows a retainage entry and a two-job WIP schedule using these lines.

## How to use it

1. Open `chart-of-accounts.csv` and line up the 5000s with the cost lines on
   your estimates. Add or rename lines so the two match exactly.
2. Keep overhead (office wages, shared trucks, insurance) in the 6000s, even
   when it feels like part of every job.
3. Import the rest. If your software uses five-digit numbers, add a zero to
   each (1110 becomes 11100).

This chart totals costs by type. Costs job by job come from your estimating or
project tool, which is also where the WIP schedule figures come from.

## Entries these lines are built for

A 50,000.00 progress bill with 10% retainage:

| Line | Debit | Credit |
|---|---|---|
| 1100 Accounts receivable | 45,000.00 | |
| 1110 Retainage receivable | 5,000.00 | |
| 4010 Contract revenue | | 50,000.00 |

A sub's 12,000.00 bill with 10% held back: debit 5030 Subcontractors
12,000.00, credit 2010 Accounts payable 10,800.00 and 2020 Retainage payable
1,200.00.

Month-end WIP adjustment, per job: revenue earned is contract price times
percent complete (cost to date divided by estimated total cost). If billed to
date is higher, the excess goes to 2100 with a matching reduction in 4010. If
it is lower, the shortfall goes to 1200 with a matching increase in 4010. All
amounts here are illustrative.

## Checks at month end

- 1110 falls as jobs close. A balance that keeps growing usually means closeout
  paperwork has stalled.
- 1200 and 2100 come from this month's WIP schedule, not last month's.
