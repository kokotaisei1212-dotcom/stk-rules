# STK permission rules

These rules are published and signed by [stk-evidence.com](https://stk-evidence.com/rules).

Which actions of an AI in a conversation with a customer a law gives to a person, by jurisdiction, with each law's citation. STK's reading of the law, not legal advice.

- `data/rules.txt`: the current version's full text, as `GET https://api.stk-evidence.com/v1/rules` gives it.
- `data/versions.json`: every version, each with STK's signature (`kid`, `sig`), from `GET https://api.stk-evidence.com/v1/rules?history=1`. Check a signature with [stk_verify.py](https://stk-evidence.com/stk_verify.py) and the keys at `GET https://api.stk-evidence.com/v1/rules?keys=1`.
- `data/actions.json`: each action, its side (`ai` or `person`), its laws, jurisdictions and official texts.
- `data/laws.json`: each law, by jurisdiction and subject, with its anchor on https://stk-evidence.com/rules.

Updated from those addresses each time the site is published (`.github/workflows/update.yml`). Licence: [CC BY 4.0](LICENSE). Name STK as the source and say what you changed.
