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

![Terminal Demo](https://github-production-user-asset-6210df.s3.amazonaws.com/315022074/633461046-384a3d80-bcff-4d8d-ae9a-89c158640525.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAVCODYLSA53PQK4ZA%2F20260809%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20260809T225149Z&X-Amz-Expires=300&X-Amz-Signature=4703d4c8d9c83d78247d3186cf0c46bcd68b22edffccbf6b955520d8774c9a57&X-Amz-SignedHeaders=host&response-content-type=image%2Fpng)

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

![Telegram Alert]([images/telegram_hit.png](https://github-production-user-asset-6210df.s3.amazonaws.com/315022074/633461204-94969d18-2121-45e8-8b10-51db450a3bab.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAVCODYLSA53PQK4ZA%2F20260809%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20260809T225313Z&X-Amz-Expires=300&X-Amz-Signature=69a4e713ceffd9a9205e9e3bec29c873190c33141b932d052901557fd4817349&X-Amz-SignedHeaders=host&response-content-type=image%2Fpng))


## Tools Available

For access to the full exploitation toolkit, contact us:

📩 Telegram: [@chainIntelligence0](https://t.me/chainIntelligence0)
📢 Channel: [coldcardeenum_tools](https://t.me/coldcardeenum_tools)
🐦 Twitter: [@ChainIntelTech](https://x.com/ChainIntelTech)

---

## Disclaimer

This research is for educational and recovery purposes only. Unauthorized access to others' wallets is illegal.
