# 水务环保工程技能库（试用版）

面向水务、环保、工程造价与工程管理一线的 Agent 技能集合，供 Claude Code、Codex、Cursor、Qoder、OpenCode 等工具安装使用。

每个技能都以 `SKILL.md` 组织：写清适用场景、判断口径、执行流程与输出形态。试用版给方法与结构，完整版给可执行的脚本、知识库与成品模板。

## 安装

```bash
# 列出本仓库全部技能
npx skills add fengqing008/water-works-skills --list

# 全部安装到 Claude Code
npx skills add fengqing008/water-works-skills -a claude-code

# 只装一个技能到 Qoder
npx skills add fengqing008/water-works-skills --skill wastewater-microscopy-preview -a qoder
```

要求 Node.js 22.20 及以上。

## 技能清单

| 技能 | 解决什么问题 |
|---|---|
| [settlement-audit-preview](skills/settlement-audit-preview/SKILL.md) | 工程结算资料核对、工程量复核口径、审减风险排查、审核报告结构 |
| [acceptance-filing-preview](skills/acceptance-filing-preview/SKILL.md) | 竣工验收条件核对、验收组织、备案材料与 15 日时限、报告框架 |
| [wastewater-microscopy-preview](skills/wastewater-microscopy-preview/SKILL.md) | 镜检判读流程、指示生物与工况对照、异常诊断路径 |

## 试用版与完整版

| 项目 | 试用版（本仓库） | 完整版 |
|---|---|---|
| 覆盖范围 | 方法与结构 | 全量知识库 + 脚本 + 模板 |
| 是否可出成品 | 需人工整理 | 可直接出 Word / Excel / HTML |
| 更新 | 不定期 | 随规范与政策更新 |

完整版在 SkillPay 货架获取，检索「水务环保技能工坊」。购买后由平台发放压缩包，无需人工对接。

## 技术说明

- 技能遵循 `skills` CLI 的目录约定：`skills/<name>/SKILL.md`
- `description` 字段包含中英文触发词，决定智能体何时调用
- 试用版不含任何脚本与私有数据，可放心安装查看

## 授权

本仓库内容可免费用于学习与个人工作，**禁止转售、禁止整体搬运到付费产品**。详见 [LICENSE](LICENSE)。

## 反馈

发现问题请提 Issue，注明技能名与具体场景。涉及具体工程的判断，请以现行规范与属地主管部门要求为准。
