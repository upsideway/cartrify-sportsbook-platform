# Integration guide — what an operator needs before a sportsbook goes live

This is the checklist we run with every operator. It is published because most delays in this
market are not technical — they are unglamorous prerequisites that nobody listed at the start.

Nothing here requires you to use Cartrify. If it helps you launch properly on any platform, that is
a good outcome.

---

## 1. Licence and corporate entity

| Item | Notes |
|---|---|
| Operating licence | Held by your local entity, or in application. Nigeria (NLRC / state lotteries), Ghana (Gaming Commission), Kenya (BCLB) and most African jurisdictions license the **operator**, not the software vendor. |
| Corporate documents | Certificate of incorporation, directors, shareholding, registered address, tax identification. |
| Licence conditions | Stake limits, payout ratios, advertising restrictions, reporting frequency, player complaint handling. These become product requirements — read them before build, not after. |
| Data protection | Player data handling, retention and disclosure rules. Regulators increasingly ask who can see player data and where it is stored. |
| AML policy | Customer due diligence tiers, thresholds, suspicious transaction reporting, record retention. |

**Timeline reality:** licensing runs on the regulator's clock, not yours. Software can be ready in
three weeks; the licence frequently cannot.

---

## 2. Money in and money out

This is where launches fail. Before go-live you need, for every rail you intend to run:

- **A merchant account or gateway contract** in your entity's name (not a personal account).
- **Settlement timing** — T+0, T+1, or weekly. It sets your working capital requirement.
- **Chargeback and dispute rules** for card; reversal handling for mobile money.
- **Agent cash-in / cash-out** — float funding, agent commission, reconciliation, and what happens
  when an agent's float runs dry mid-match.
- **Withdrawal policy** — verification requirements, manual review thresholds, and the payout
  window you actually commit to. Players do not forgive a broken promise here.
- **Reconciliation** — one report per rail per day that ties gateway settlement to your ledger. If
  you cannot reconcile, you cannot audit, and you cannot scale.

Rails that matter in African markets, as an example: M-Pesa, MTN MoMo, Airtel Money, Paystack, OPay, Budpay, Moniepoint,
Palmpay, Flutterwave, plus bank transfer and USDT.

---

## 3. Odds and markets

| Decision | What it changes |
|---|---|
| **Feed provider** | LSports, SportsRadar, Betradar, Kambi, or a compilation feed. Contracted directly with the provider — the feed is usually a separate cost from the platform. |
| **Latency** | In-play prices that arrive late are a liability, not a product. Ask for feed latency in writing. |
| **Market depth** | Football 1X2 is table stakes. Asian handicap, over/under, correct score, player props and outrights are what separates a serious book. |
| **Settlement source** | Who decides a void, an abandoned match, a stat correction — and how fast. Ambiguity here produces player complaints and regulator letters. |
| **Risk controls** | Per-market liability limits, stake limits by player tier, exposure monitoring across the whole book, and a way to pull a market fast. |

---

## 4. Platform and operations

- **Admin access** — who can move odds, void a bet, adjust a limit, credit a wallet. Every action
  logged with an operator identity. Shared logins are how fraud hides.
- **KYC** — document capture, liveness, duplicate-account detection, and the tier thresholds that
  decide when a player must verify before withdrawing.
- **Player support** — a queue your team can work, with bet history and wallet state visible on the
  same screen.
- **Monitoring** — feed outage, payment failure rate, settlement lag, and a human who is woken up
  when they break.
- **Reporting** — daily GGR, deposits, withdrawals, active players, and the regulator report in the
  format they asked for.

---

## 5. Launch checklist (the short version)

- [ ] Licence held or application lodged, with conditions mapped to product behaviour
- [ ] Corporate and KYC documents accepted by the payment providers
- [ ] At least two payment rails live, one of them mobile money
- [ ] Odds feed contracted, latency tested in-play
- [ ] Settlement and void rules written down and agreed
- [ ] Agent float funded, commission and reconciliation signed off
- [ ] Withdrawal promise defined (amount, window, verification) and stress-tested
- [ ] Support queue staffed for the hours your players actually bet
- [ ] Regulator report produced once, manually, before go-live — not discovered afterwards
- [ ] Rollback plan: what you do at 21:00 on a Saturday when payments stop

---

## Questions

**info@cartrify.com** · [cartrify.com](https://cartrify.com)

Cartrify is the white-label sportsbook platform behind NaijaBet. A fixed monthly licence fee in
USD, no revenue share, live in three weeks.
