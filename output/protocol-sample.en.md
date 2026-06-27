# protocol-sample 翻訳結果（JA→EN）

- Mode: C（Protocol 抜粋／フル工程）
- 方向: JA→EN
- ステータス: **DRAFT**（HITL 承認前。承認＝git commit で CONFIRMED）
- モデル: Claude（本セッション／Claude Code・Anthropic API 経由）
- 検証: 逆翻訳投票 3体 → 3/3 不一致 → 指摘反映済み

---

## 確定訳（DRAFT・DW 反映後）

This clinical trial aims to evaluate the efficacy and safety of the investigational product (IP) ABC-123 in subjects. <!-- src: protocol-sample.md L1 -->

If a serious adverse event (SAE) occurs within 24 hours after the first administration of the investigational product (IP), the subject must promptly contact the investigator. <!-- src: protocol-sample.md L2 -->

The investigator shall report all adverse events (AEs) to the sponsor and, where necessary, seek the judgment of the Data and Safety Monitoring Board (DSMB). <!-- src: protocol-sample.md L3 -->

Deviations from this protocol are not permitted except where the prior approval of the sponsor has been obtained. <!-- src: protocol-sample.md L4 -->

---

## DW 検証の記録（監査証跡用）

逆翻訳投票（独立3体）→ **3/3 不一致**。検出・修正:

| 指摘 | 検出 | 対応 |
|---|---|---|
| 第1文「本治験」が "This **study**" ＝禁止訳"study"単独 | 3/3（全会一致） | "This **clinical trial**" に修正 |
| "is intended to" が「目的とする」よりやや弱い | 1/3 | "aims to" に修正 |
| 効果安全性評価委員会→DSMB が Protocol 正式名称と一致するか | 1/3 | ⚠️要確認（用語集は DSMB を指定。Protocol 定義名と突合を推奨） |

## ⚠️ 人間レビュー（HITL）への申し送り
- 委員会名 DSMB が当該 Protocol の正式英名と一致するか確認（verifier 3 指摘）。
- 承認後に本ファイルを git commit すれば CONFIRMED（＝監査証跡確定）。
