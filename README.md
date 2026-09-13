# dietrichgebert-ponytail

DSH 技能分组仓：**dietrichgebert-ponytail**

- **上游**：https://github.com/DietrichGebert/ponytail
- **说明**：本仓内容以本机实际使用的版本为准（可能已对上游做过改名/翻译/本机适配）。
  上游只作祖先与对照——**不要用上游覆盖本地**（见 MyAI `docs/adr/0006`）。

## 内容

- `ponytail`
- `ponytail-audit`
- `ponytail-debt`
- `ponytail-gain`
- `ponytail-help`
- `ponytail-review`

由 `dsh-extensions/install-skill.sh` 软链进 `~/.dsh/skills/`。

## 本仓的本地改动（相对上游）

上游把六个技能放在嵌套的 `skills/` 目录里，与「分组仓技能放组根」的约定不符，
本仓按其他组的先例把 `skills/*` 拍平到组根（`git mv skills/<name> .`）。
除这一处结构改动外，技能正文与上游一致（MIT）。
