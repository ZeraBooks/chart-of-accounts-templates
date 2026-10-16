# Chart of accounts templates

A small business chart of accounts is the numbered list of every account the
books post to, grouped by type: assets, liabilities, equity, income, cost of
sales and operating expenses. Each industry then adds a few lines of its own,
such as a trust account and the matching client liability for a law firm. The
CSVs here give that layout for five industries.

Each file uses the same five columns (Number, Name, Type, Detail, Notes) and the
same number ranges.

| Range | Type |
|---|---|
| 1000s | Assets |
| 2000s | Liabilities |
| 3000s | Equity or net assets |
| 4000s | Income |
| 5000s | Cost of sales |
| 6000s | Operating expenses |

| Folder | Built around | Guide |
|---|---|---|
| [`nonprofits/`](nonprofits/) | Gifts split by donor restriction, expenses split by function for Form 990 Part IX | [Bookkeeping for nonprofits](https://www.zerabooks.com/bookkeeping-for-nonprofits) |
| [`restaurants/`](restaurants/) | Food and beverage sales and cost, delivery apps, tips and sales tax held for others | [Bookkeeping for restaurants](https://www.zerabooks.com/bookkeeping-for-restaurants) |
| [`law-firms/`](law-firms/) | The trust account and the client liability it must equal, legal fees by type | [Bookkeeping for law firms and trust accounts](https://www.zerabooks.com/bookkeeping-for-law-firms) |
| [`contractors/`](contractors/) | Job costs on the lines you bid, retainage, over and under billings | [Bookkeeping for contractors](https://www.zerabooks.com/bookkeeping-for-contractors) |
| [`property-management/`](property-management/) | Trust and operating accounts, owner funds and tenant deposits held | [Bookkeeping for property management](https://www.zerabooks.com/bookkeeping-for-property-management) |

Each folder's README explains the lines that are specific to that industry.
The account names are generic and contain no real company data.

## How to use these files

1. Open the industry's `chart-of-accounts.csv` in a spreadsheet.
2. Delete the lines you don't need and rename the placeholders the folder
   README points out.
3. Import the rest into your accounting software. If it uses five-digit
   numbers, add a zero to each.

## License

The content and data in this repository are licensed under
[CC BY 4.0](LICENSE). Free to use and adapt with credit to ZeraBooks.

Maintained by [ZeraBooks](https://www.zerabooks.com).
