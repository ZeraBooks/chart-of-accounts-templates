# Restaurant chart of accounts (CSV)

A restaurant chart of accounts splits sales and costs the way the kitchen and
bar run: food sales against food cost, beverage sales against beverage cost,
delivery app sales on their own line with the commissions as an expense, and
card tips and sales tax as liabilities because they belong to staff and the
state. With those lines in place, prime cost (food and drink cost plus all
labor) reads straight off the profit and loss. The worked April in ZeraBooks'
[bookkeeping for restaurants](https://www.zerabooks.com/bookkeeping-for-restaurants)
guide uses the same structure.

## How to use it

1. Open `chart-of-accounts.csv` and delete what doesn't fit (1020 if you run
   payroll from operating, 5030 if packaging goes with paper goods).
2. If the bar is a big part of the business, split 4020 into liquor, beer and
   wine, and split 5020 the same way so each pour cost can be measured.
3. Import the rest. If your software uses five-digit numbers, add a zero to
   each (4010 becomes 40100).

## Entries these lines are built for

| Event | Debit | Credit |
|---|---|---|
| Card batch with tips | 1010 Operating checking | 4010 or 4020 sales (pre-tax), 2200 Sales tax payable, 2100 Tips payable |
| Tips paid out through payroll | 2100 Tips payable | 1010 or 1020 checking |
| Monthly delivery app gross-up from payout reports | 6310 commissions, 6400 promotions, 4900 refunds | 4030 Delivery app sales |
| Food inventory fell over the month | 5010 Food cost | 1200 Food inventory |
| Gift card sold | 1010 Operating checking | 2300 Gift cards outstanding |
| Sales tax paid to the state | 2200 Sales tax payable | 1010 Operating checking |

Food cost for the month is opening food inventory plus purchases minus closing
inventory. The count on the last night of the month is the one figure no
statement shows, so book purchases to 5010 and 5020 as they happen and post the
change in inventory once the count is in.

## Checks at month end

- 2100 Tips payable is close to zero after the last pay run.
- 2200 Sales tax payable equals tax collected less tax remitted.
- 4030 Delivery app sales equals the order subtotals on the payout reports,
  not the deposits.
