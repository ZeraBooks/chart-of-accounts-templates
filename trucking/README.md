# Trucking company chart of accounts (CSV)

A trucking company's chart of accounts should split revenue into linehaul, fuel
surcharge and accessorials, and put the costs that move with miles (fuel,
driver pay, tolls, repairs, tires) in cost of sales. Then the profit and loss
shows revenue and cost per mile, and the fuel surcharge can be compared with
what fuel actually cost. It also needs a fuel tax payable line for the
quarterly return, and optional factoring lines if invoices are sold to a
factor. ZeraBooks' guide to
[bookkeeping for trucking](https://www.zerabooks.com/bookkeeping-for-trucking)
covers the month-end routine for these accounts.

## How to use it

1. Open `chart-of-accounts.csv`. Delete the factoring lines (1110, 2100, 5070)
   if you do not factor, and delete 5030 and 2310 if you have no contractors.
2. Keep dispatch and office costs in the 6000s. Costs that rise and fall with
   miles stay in the 5000s.
3. Import the rest. If your software uses five-digit numbers, add a zero to
   each (5010 becomes 50100).

Costs per truck or per load come from your fleet or dispatch software. This
chart totals costs by type.

## Entries these lines are built for

A 10,000.00 freight invoice sold to a factor with 90% advanced and a 2% fee
(illustrative):

| Line | Debit | Credit |
|---|---|---|
| 1100 Accounts receivable | 10,000.00 | |
| 4010 Linehaul revenue | | 10,000.00 |

When the factor advances 9,000.00 and charges 200.00:

| Line | Debit | Credit |
|---|---|---|
| 1010 Operating checking | 9,000.00 | |
| 5070 Factoring fees | 200.00 | |
| 1110 Factoring reserve receivable | 800.00 | |
| 1100 Accounts receivable | | 10,000.00 |

Fuel purchased on a card and paid later: debit 5010 Fuel, credit 2400 Business
credit card. The card payment from checking is a transfer to 2400, not an
expense.

## Checks at month end

- 1110 should fall as customers pay the factor. A balance that keeps growing
  means invoices are unpaid past the reserve release date.
- 2200 should agree with the fuel tax return worksheet for the quarter.
- 5010 divided by miles driven is miles per gallon turned into dollars per
  mile. A sudden jump on one truck is usually a fuel card used on another
  vehicle.

## FAQ

### Is a fuel surcharge revenue or a reduction of fuel cost?

Revenue. It is billed to the customer, so it belongs in income. Keeping it on
its own line (4020) from the fuel expense (5010) shows whether the surcharge
covers fuel.

### How do I record a factoring fee?

The fee is an expense, usually at the time of the advance. The advance itself is
not revenue, because the revenue was recorded when the invoice was issued.
Any reserve the factor holds stays a receivable until it is released.

### Do I send a 1099-NEC to owner-operators?

For payments made from 2026, yes for any contractor that is not a corporation
and was paid $2,000 or more in the year, under the current IRS instructions.
Collect a Form W-9 before the first payment.
