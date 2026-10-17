# 🛡️ Perp Risk Guard

**A free, single-file futures risk calculator. Spend 20 seconds before every entry — block 90% of liquidations.**

No install · No build · No signup · Works offline · 中文 / EN built-in

> 🔗 **Live demo:** <https://haolinsong32-lang.github.io/perp-risk-guard/> — the demo IS `index.html`, the whole app is one file.

---

## Why

Most futures blow-ups are not "wrong direction" — they are **wrong size, wrong stop, or a grid that overlaps the liquidation price**. This tool forces the check *before* you click the buy button.

## Features

| Module | What it checks / does |
|---|---|
| ① Account & Direction | Equity, leverage, per-trade risk %, maintenance margin rate |
| ② Entry / Stop / Liquidation | Isolated-margin liquidation price, risk-based position sizing, "stop must fire before liquidation" iron rule |
| ③ Grid ladder | Pending orders auto-snap to 05-ending levels; **fails hard if the liquidation price falls inside the grid range** |
| ④ T1 / T2 / T3 scaled TP | Ladder take-profit with stop-move, OCO reminders, total-PnL preview |
| ⑤ Kelly check (optional) | Full & half-Kelly sizing from your historical win-rate and payoff ratio |
| 📋 Copy plan | One click → paste your full trade plan into notes or a group chat |

## The Pass-It-On Challenge 🔥

This tool is **free forever**. In exchange, when it saves your account once:

1. ✅ Run one pre-entry check with it
2. 📸 Screenshot your "✅ Risk check passed" result
3. 🤝 Send it to one trading friend and invite them to continue the chain

**Every new node = one fewer blown account.** That is the whole business model.

## Spread & earn 30% (optional)

Want to do more than pass it on? The paid **Pro edition** (batch grid A/B/C compare + plan archive + trade journal & review) is live at **[pay.suka.net.cn](https://pay.suka.net.cn)** — 9 USDT, instant delivery via USDT multi-chain payment or redeem code. Affiliates earn **30% on every sale** (StoneVast Node Program) — contact haolinsong32@gmail.com to get your referral codes.

## Run locally

1. Download `index.html`
2. Double-click it. Done.

Zero dependencies, zero network calls — data never leaves your browser. Language preference is remembered (localStorage); deep-link with `?lang=en` or `?lang=zh`.

## Roadmap

- [x] Single-file free edition (this repo)
- [x] Pro edition: batch grid A/B/C compare, plan archive, trade journal & review — [get it here](https://pay.suka.net.cn) (9 USDT)
- [ ] Live exchange price fetch (opt-in)

## License

MIT — free to use, modify and redistribute. The commercial Pro edition is sold separately.

## Disclaimer

Educational tool with a simplified isolated-margin model. Liquidation prices and fees vary by exchange — **always trust your exchange's numbers**. Nothing here is financial advice. Trading futures is risky; never risk what you cannot afford to lose.
