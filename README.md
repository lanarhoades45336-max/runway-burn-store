# Runway & Burn Kit

Two small, dependency-free tools for one question: **how long can your money last, and what is quietly draining it?**

No account. No telemetry. Plain Python you run yourself.

## What you get

**`runway.py` — how many days of money do you have left?**
Turns your cash, monthly cost and income into a concrete number: your runway in days. Add `--simulate` and it runs a Monte-Carlo over irregular income, so you see a survival rate instead of a single guess.

**`subscriptions.py` — what is quietly draining you?**
Reads a bank/statement CSV and finds the recurring charges you forgot about, with a monthly and annualized total. Handles real, messy statements (capitalised headers, `$`, quotes, refunds in parentheses).

## Try it

```bash
python3 runway.py --cash 6000 --monthly-cost 2500 --monthly-income 3000
python3 runway.py --cash 6000 --monthly-cost 2500 --income-mean 3000 --income-std 1500 --simulate
python3 subscriptions.py --csv statement.csv
```

Both scripts print a readable report by default and machine-readable JSON with `--json`.

## Price and how to buy

**US$ 19.** Pay in native ETH, USDC or USDT on Ethereum — scan the QR or tap the link on the product page:

**https://lanarhoades45336-max.github.io/runway-burn-store/runway---burn-kit.html**

Delivery is automatic: the files appear at a private link right after the payment confirms.

## Honesty note

These tools do arithmetic on numbers you give them. They do not predict markets and they do not manage your money. They make one thing clear: your runway, and your recurring burn. That is all they claim.
