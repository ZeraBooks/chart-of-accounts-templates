# Law firm chart of accounts (CSV)

A law firm's chart of accounts is a normal business chart plus a matched pair:
the IOLTA trust bank account (an asset) and Client trust funds (a liability for
the same amount, because every dollar in trust is owed to a client).

Add a Client costs advanced asset for fees paid on a client's behalf, legal fees
split by hourly, flat and contingency, and a capital and draw pair for each
partner. ZeraBooks' guide to
[bookkeeping for law firms](https://www.zerabooks.com/bookkeeping-for-law-firms)
covers the trust rules these lines are built around and a month of trust
activity.

## How to use it

1. Open `chart-of-accounts.csv`. Rename the 3010 to 3040 partner lines and add
   a pair for each further partner. A sole practitioner can use one Owner
   capital and Owner draws pair instead.
2. Delete 1030 if you hold every client's money in the pooled IOLTA account.
3. Keep client-by-client balances in your trust ledger or practice management
   software. 2100 holds the total; the client ledgers hold the detail.
4. Import the rest. If your software uses five-digit numbers, add a zero to
   each (1020 becomes 10200).

## How trust money moves through these lines

| Event | Debit | Credit |
|---|---|---|
| Retainer deposited to trust | 1020 IOLTA trust account | 2100 Client trust funds |
| Settlement paid out to the client from trust | 2100 Client trust funds | 1020 IOLTA trust account |
| Earned fee leaves trust | 2100 Client trust funds | 1020 IOLTA trust account |
| The same fee arrives in operating | 1010 Operating checking | 4010, 4020 or 4030 Legal fees |
| Filing fee paid for a client from operating | 1200 Client costs advanced | 1010 Operating checking |
| Client repays the filing fee | 1010 Operating checking | 1200 Client costs advanced |

Treating client costs advanced as an asset means a 400.00 filing fee never
shows up as both an expense and income.

## The monthly three-way check

These three figures must agree on the last day of every month:

1. The trust bank statement's closing balance, after uncleared items.
2. 1020 (plus 1030 if used) in the books, which must also equal 2100.
3. The total of every client ledger.

No client ledger may be negative. Check your own state's version of ABA Model
Rule 1.15 for record keeping and reconciliation requirements.

## FAQ

### Is money in a law firm's trust account the firm's income?

No. Client money in the trust or IOLTA account belongs to the client until a fee
is billed and earned. The earned fee is then transferred to operating and
recorded as revenue there; leaving it in trust is commingling.

### Who gets the interest on an IOLTA account?

The bank pays IOLTA interest to the state's IOLTA program, which funds legal
aid, so it is never firm income. A large or long-held sum for one client goes in
its own interest-bearing trust account, and that interest belongs to the client.

### Is bookkeeping for a solo lawyer different from a law firm?

Not in the rules. A solo lawyer holding client money needs the same trust
account, the same liability and the same monthly three-way reconciliation as a
large firm; the difference is volume.
