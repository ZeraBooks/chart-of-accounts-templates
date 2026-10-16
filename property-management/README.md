# Property management chart of accounts (CSV)

A property management company needs two sets of lines kept apart: the company's
own operating account and income (management fees, leasing fees), and the trust
account that holds other people's money, matched by two liabilities, owner
funds held and tenant security deposits held. When the books are right, the
trust bank balance equals every owner's balance plus every deposit held.
ZeraBooks' guide to
[bookkeeping for property management](https://www.zerabooks.com/bookkeeping-for-property-management)
works through a month of a 12-unit trust account on this layout.

## How to use it

1. Open `chart-of-accounts.csv`. Rename 2210 and 2220 to your owners and add a
   child under 2200 for each one.
2. Delete 2400 and the 5000s if you don't hold reserves or bill maintenance.
3. Import the rest. If your software uses five-digit numbers, add a zero to
   each (2210 becomes 22100).

This chart is for a manager. A landlord who owns the buildings uses rent,
repairs, insurance and property tax lines by property instead of the trust
lines.

## How money moves through these lines

| Event | Debit | Credit |
|---|---|---|
| Rent collected for Owner A | 1020 Trust checking | 2210 Owner funds held: Owner A |
| New tenant's security deposit | 1020 Trust checking | 2100 Tenant security deposits held |
| Repair paid from trust for Owner A | 2210 Owner funds held: Owner A | 1020 Trust checking |
| Management fee earned on Owner A's rent | 2210 Owner funds held: Owner A | 1020 Trust checking |
| The same fee arriving in operating | 1010 Operating checking | 4010 Management fees |
| Owner distribution paid to Owner A | 2210 Owner funds held: Owner A | 1020 Trust checking |

Owner distributions are never an expense of the management company. They
reduce what the trust owes that owner. 3020 is only for the company's own
owners.

## The month-end check

Before paying owners: trust bank closing balance (after uncleared items) =
2100 + every child of 2200 + 2300 + 2400. If it doesn't, find the difference
first. Many states require licensed managers to keep these funds in a separate
account; check your real estate commission's rules.
