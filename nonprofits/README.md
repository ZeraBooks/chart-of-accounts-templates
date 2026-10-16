# Nonprofit chart of accounts (CSV)

A small nonprofit needs a business-style chart of accounts with two extra
splits: income divided by donor restriction (with or without), and expenses
divided by function (Program, Management and general, Fundraising), so the
Form 990 Part IX columns come straight from the books. This file sets up both
splits, plus refundable advances for conditional grants and in-kind
contributions. ZeraBooks' guide to
[bookkeeping for nonprofits](https://www.zerabooks.com/bookkeeping-for-nonprofits)
walks a full month of these lines with a fictional literacy charity.

## How to use it

1. Open `chart-of-accounts.csv` in a spreadsheet.
2. Rename 4110 and 4120 to your actual restricted grants or purposes, one line
   each, and add more children in the 4100s as new restricted gifts arrive.
3. Delete lines you won't use (for example 2400 if you hold no ticketed events).
4. Import into your accounting software. If it uses five-digit numbers, add a
   zero to each (1010 becomes 10100).

## The lines that make it a nonprofit chart

| Lines | Why they are there |
|---|---|
| 3010, 3020 | Net assets replace owner equity, split by donor restriction |
| 4110, 4120 | One line per restricted grant, so a funder asking how its money was spent gets that grant's own lines |
| 4910, 4920 | Releases from restriction. When restricted money is spent on its purpose, debit 4910 and credit 4920 for the same amount |
| 2300 | Cash received on a conditional grant (a barrier plus a right of return) waits here until the condition is met |
| 4300 | Donated goods and qualifying services at fair value, entered by journal entry because they have no bank line |
| 6040, 6140, 6240 | To allocate lines. Shared salaries and rent sit here during the month, then one entry splits them by timesheets and floor space |
| 4400, 5010 | Event tickets: the fair value of the dinner is event revenue and its cost is a direct benefit to donors; the rest of the ticket is a contribution |

## Checks at month end

- Every To allocate line is zero.
- 4910 plus 4920 is zero.
- Each restricted child in the 4100s, less the releases for it, matches what
  the funder still expects you to spend.

This is a starting point, not tax advice. Your auditor or 990 preparer may ask
for extra lines, such as a separate line per government award.
