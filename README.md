# Coldcard RNG Vulnerability — Research & Tooling

**Chain Intelligence** | [@ChainIntelTech](https://x.com/ChainIntelTech)

---

## Background

In July 2026, a firmware bug in Coldcard hardware wallets collapsed wallet entropy from 256 bits to ~40 bits. Attackers exploited this to drain 1,700+ BTC (~$110M) across 4 waves.

We reverse-engineered the exact attack chain.

---

## Our Research

- ✅ Firmware bit-exact Yasmarang PRNG reproduction
- ✅ 8,450+ verified victim addresses collected
- ✅ 340 confirmed wallet matches
- ✅ Full parameter coverage (RTC, SSR, UID, kpad_a/b, chip_skip, mixer_skip)
- ✅ Offline UTXO matching (47M scripts)
- ✅ Multi-coin support (BTC, BCH, LTC, DOGE)

---

## Proof of Work

![Terminal Demo](terminal_output.png)
COLDCARD ENUM TOOLS v2.1 — LIVE SCAN
Engine: Yasmarang PRNG (firmware bit-exact port)

Configuration:
RTC range : 0-100
UID blocks : 0x1a, 0x1b, 0x23, 0x46
Profile : retail-first-boot
BIP path : m/84'/0'/0'/0/0

SCANNING IN PROGRESS
[████████████████░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░] 33%

[!] HIT DETECTED — Verifying...
🔥 CONFIRMED: bc1q...
🔑 wood bundle convince into what option diesel dutch...
Status: VERIFIED — Matched in victim database


---

## Tools Available

For access to the full exploitation toolkit, contact us:

📩 Telegram: [@chainIntelligence0](https://t.me/chainIntelligence0)
📢 Channel: [coldcardeenum_tools](https://t.me/coldcardeenum_tools)
🐦 Twitter: [@ChainIntelTech](https://x.com/ChainIntelTech)

---

## Disclaimer

This research is for educational and recovery purposes only. Unauthorized access to others' wallets is illegal.
