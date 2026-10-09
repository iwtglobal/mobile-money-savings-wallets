# Savings Product Checklist

Design checklist for **mobile money savings wallets** and goal-based pots on an agent-capable platform.

## 1. Product decisions to lock early

| Decision | Options to compare |
|----------|-------------------|
| Pot count | One default pot vs many named pots |
| Lock type | Open / soft lock / hard lock / mixed |
| Funding paths | Main wallet only vs direct agent cash-in vs salary credit |
| Withdrawal paths | Back to main wallet only vs limited bill pay from pot |
| Visibility | App + USSD + agent vs app-only (usually too narrow) |
| Incentives | None / milestone bonus / partner-funded cashback (licence-checked) |

## 2. Ledger and limits

- [ ] Each pot has its own ledger account under the customer entity
- [ ] Combined pot + main wallet balances respect KYC tier caps
- [ ] Transfers between pots are posted as real entries (auditable)
- [ ] Fees (if any) post as separate fee lines, not hidden netting
- [ ] Reversals of failed cash-in never leave orphan pot credits

## 3. Customer communication

- [ ] Goal create/edit copy is clear in the customer's language
- [ ] Unlock date and early-exit terms shown before confirm
- [ ] Progress notifications are opt-in or frequency-capped
- [ ] Statement history shows pot name on each line

## 4. Agent banking adjacency

- [ ] Agent can explain and cash into the pot without a smartphone demo
- [ ] Receipt prints or SMS confirms pot name and new pot balance
- [ ] Agent incentives (if any) do not encourage unsuitable "lock" sales
- [ ] Dispute path for "I meant main wallet" mis-routing

## 5. Launch readiness

- [ ] Regulatory product approval / notification where required
- [ ] Dormancy and unclaimed funds policy documented
- [ ] Ops runbook for stuck locks and bereavement access
- [ ] KPI definitions: active pots, funded pots, early exits — no vanity vanity metrics

## Related

See the main [README](../README.md). Product context: [mobile money platform with merchant payment](https://evdsystem.com/mobile-money-platform-with-merchant-payment/).
