# 🚘 Vulnerable Vehicles and Key Fob Resynchronization Methods
A curated, navigable reference of vehicle models reported in a publicly circulated list as vulnerable to custom Flipper Zero firmware that can desynchronize key fobs. For each make/model this document records whether a free DIY resynchronization method is credibly available and short guidance for owners. Use this only for lawful, owner-led recovery and diagnosis.

**High-level context:** public reporting indicates custom Flipper Zero firmware exists that replays or reuses known rolling-code weaknesses and can desynchronize legitimate fobs. For owners, this document records whether free resynchronization methods are credibly available.

![vulnerableListFromCFWDev](https://github.com/user-attachments/assets/f66c25d1-8d04-442e-9afc-30e9b2aab924)


---

## 📋 Table of contents
- Scope and purpose
- Quick summary & credibility notes
- Vulnerable vehicles (compact table)
- Per-manufacturer details (expandable)
- General DIY resynchronization (high level)
- Safety, legal, and disclaimers
- References (APA)

---

## 📏 Scope and purpose
This document collects a public list of vehicle models that have been reported in circulation as *potentially* vulnerable to custom Flipper Zero firmware that interferes with key fob rolling-code interactions. For each entry I note whether a free DIY resynchronization procedure is credibly available from manufacturer documentation or well-established community sources. Where no credible free method exists I mark the entry accordingly.

This is not an exhaustive security analysis. Vehicle firmware and immobilizer implementations vary by market, trim, and year. Always verify with the vehicle manufacturer or an authorized locksmith/technician.

---

## ✏️ Quick summary & credibility notes
- **What is being reported:** custom firmware distributed in underground markets can replay or substitute single rolling-code transmissions. That process may cause the vehicle and original fob to fall out of sync.
- **Manufacturer responses:** automakers and Flipper Devices have publicly stated they are evaluating reports and that the device alone has limitations. Independent reporting and vendor statements disagree on scope.
- **Practical effect on owners:** older vehicles using legacy rolling-code schemes (e.g., KeeLoq era systems) are more likely to be recoverable with owner procedures. Modern vehicles typically require dealer/diagnostic tools.

---

## 🔓 Vulnerable vehicles (compact table)
Use this as a quick index. See the expanded sections below for notes.

| # | Manufacturer | Model(s) (reported) | Years (as reported) | Free DIY resync? | Short note |
|---:|---|---|---:|---:|---|
| 1 | KIA | Carens, Forte, Rio, X-Line, Getz, Ceed, Picanto, Optima, Venga, Sorento, Sportage, Cerato, Carnival, Magentis, Soul, Sedona, K-series (KX, KRX), Stonic | up to 2025 | Mostly no | Older models sometimes have ignition/button re-learn. Most recent models require programming tools. |
| 2 | HYUNDAI | Accent, Solaris, Verna, Getz, Avante, i-series up to i40, ix20 | up to 2025 | Mostly no | Same pattern as Kia. |
| 3 | SUBARU | Tribeca, Forester, Impreza, Outback | specific older ranges (e.g., 1998–2009) | Sometimes yes (older models) | Older models have well-documented ignition/door sequence methods. |
| 4 | FIAT / FCA | Doblo, Cronos, Ducato, Lancia, others | varied | No | No credible free method found; requires specialist tools. |
| 5 | FORD | Fiesta, Focus, C-Max, S-Max, Galaxy, Kuga, Mondeo, Explorer, Transit, Mustang, F-Series, Ranger, many others | up to 2024 | Some older yes; most newer no | Many older Fords have owner re-learn steps. Newer PATS and smart keys require dealer equipment. |
| 6 | MITSUBISHI | Pajero, Pajero Sport, ASX, Galant, Grandis, Colt, others | up to 2025 | No / depends | Uses various protocols; many require dealer tools. |
| 7 | SUZUKI | Swift, Grand Vitara, others | up to 2025 | Undetermined | Limited public data. |
| 8 | PEUGEOT / CITROËN | Wide range (2008, 207, 3008, 307, 308, 4008, 407, 5008, Partner, Berlingo, Cx series, DS series, etc.) | up to ~2018 (reported) | Mostly no | Many older PSA vehicles use rolling codes but often need dealer tools. |
| 9 | VOLKSWAGEN / SKODA / SEAT / AUDI | Many VAG models (Golf, Passat, Polo, Jetta, A4/A6/A8 etc.) | Varies; many older models up to 2008; some lines to 2015+ | Mostly no | VAG ecosystem uses varied immobilizers; earlier models sometimes re-learnable. |
| 10 | OTHERS | Jaguar, Land Rover, Lincoln, Honda (in dev), Peugeot, Citroën, etc. | up to 2025 | Varies; typically no | Newer vehicles with smart keys usually require professional equipment. |

---

## 📕 Per-manufacturer details
KIA
- Reported models: Carens, Forte, Rio, X-Line, Getz, Ceed (+Ceed ID), Picanto, Optima, Venga, Sorento, Sportage, Cerato (incl. Coupe), Carnival, Magentis, Soul, Sedona, KX/KRX/Stonic.
- Years: entries in the circulated list extend “up to 2025.”
- DIY resync: Generally not for modern models. Very old models may accept a battery-change ignition/button re-learn sequence.
- Recommended owner action: check owner manual for “key fob re-learn” or contact an authorized dealer/locksmith.

HYUNDAI
- Reported models: Accent, Solaris, Verna, Avante, i-series up to i40, ix20.
- DIY resync: Generally no for recent models. Some older models have known ignition/button re-learn flows.
- Recommended action: consult owner manual or dealer.

SUBARU
- Reported models: Tribeca, Forester, Impreza, Outback.
- DIY resync: Yes for specific older model ranges (1998–2009 / mid 2000s). Procedures typically use ignition cycles and door lock/unlock sequences.
- Credibility: well-documented legacy procedures exist in service manuals and community guides. Newer Subarus require professional tools.

FORD
- Reported models: Wide list including Fiesta, Focus, Mondeo, Kuga, Transit, F-Series, etc.
- DIY resync: Older models often yes for remote functions (2000s–early 2010s). Newer models with PATS or smart keys usually need diagnostic equipment.
- Notes: community threads and service docs list per-model key relearn procedures. Use manufacturer guidance.

Other makes (FIAT, Mitsubishi, Peugeot, Citroën, VW/Audi/SEAT/SKODA, Suzuki, Jaguar/Land Rover, etc.)
- Short view: many older models used rolling-code systems that can be manipulated with low-cost tools; however the practical ability to fully clone or reuse keys varies. Most modern vehicles use advanced two-way authentication and require dealer tools.
- Action: consult owner manual, authorized dealer, or certified automotive locksmith.

---

## 👨‍🏫 General DIY resynchronization (high level)
Only use if you are the vehicle owner or have explicit authorization. These are high-level steps that mirror common owner re-learn procedures for older vehicles. Procedures differ by model; consult the owner manual first.

1. Prepare: sit in driver seat. Close doors. Have all fobs present.
2. Enter programming mode: Insert key into ignition and cycle between OFF and ON a specified number of times within a short interval (commonly 4–10 cycles in 6–15 seconds). Vehicle may signal entry with chime or locks.
3. Program fob: press a button on the fob when prompted. Confirm via chime/locks.
4. Repeat for additional fobs.
5. Exit: turn key OFF and remove, or open door to exit programming mode.

Credibility and limits: These steps are generic. Many manufacturers publish model-specific sequences. Modern smart keys, push-button starts, and immobilizers typically do not accept simple re-learns and require dealer diagnostic tools.

---

## 🚨 Safety, legal, and operational notes
- This document is defensive. Do not use any device or firmware to intercept signals on vehicles you do not own or have explicit permission to test. Unauthorized access is illegal.
- If a DIY method is not documented by the manufacturer, assume professional programming is required. Incorrect attempts may permanently disable a fob or require replacement at cost.
- If you suspect criminal activity or theft, contact local law enforcement and your insurer.

---

## 🤔 How to use this repository
- Copy this file to README.md or keep as README.txt.
- Open issues or pull requests to:
  - Add model-specific verified resynchronization procedures with a primary source citation (service manual, dealer doc, or manufacturer support article).
  - Correct the years / model scope with supporting references.
- Label community contributions `verified` only after a supporting manufacturer or authoritative source is added.

---

## ✅ References (APA)
Hawkins, A. J. (2025, August 21). Is the Flipper Zero the next big car theft gadget? The Verge. https://www.theverge.com/cars/763446/flipper-zero-car-theft-firmware-hack-key-fob
Zhovner, P. (2025, August 22). Can Flipper Zero really steal your car? (Spoiler: NO). Flipper Devices (blog). https://blog.flipper.net/can-flipper-zero-steal-your-car/
Blanco, S. (2025, September 1). Flipper Zero Could Be the Next 'Kia Boys' Hack, or Maybe Not. Car and Driver. https://www.caranddriver.com/news/a65941613/flipper-zero-car-theft-next-kia-boys-hack/

## 🦾 Note on AI use
AI was used to perform research in the development of this project. If you are interested in exploring Manus AI (the best AI in my opinion), I invite you to use the following link so we can both get 500 credits when you sign up: https://manus.im/invitation/JJYQK0KGYUNUVL

## 💁 Support the creator
[Cash App](https://cash.app/$GhosTechRepair)
