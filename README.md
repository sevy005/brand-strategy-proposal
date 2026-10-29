# brand-strategy-proposal

**品牌策略提案公式**：从产品、消费者、竞争与企业资源事实出发，推导定位、核心价值、主推单品、传播表达与落地计划，生成可继续排版的提案正文。

适用于新品牌、品牌升级、品类进入、大单品策略，以及按既定公式写方案的任务。支持完整提案、精简提案、资料整理与已有方案修改；28页蓝图只是完整提案参考，可按项目范围调整。

## 核心方法

问题 → 机会 → 人群 → 品类 → 价值 → 产品 → 表达 → 信任 → 触点 → 验证。

- 7组策略公式：机会、定位、价值、大单品、传播、视觉与落地。
- 18个策略变量：把商业问题连接到产品、语言、识别与执行。
- 逐页提案蓝图、事实输入表、一页策略总图与审阅清单。
- 区分已核实事实、客户提供信息、分析判断与待验证假设；示例不替代真实调研。

方法源于对汤臣杰逊案例的归纳，属于独立整理的工作模板，并非该公司的官方内部模型、官方模板或授权发布内容。

## 安装

将整个仓库作为 `brand-strategy-proposal` 文件夹放入 Codex 的 skills 目录，保留 `SKILL.md`、`references/`、`assets/` 和 `agents/` 的相对位置。用户级目录可使用 `${CODEX_HOME:-$HOME/.codex}/skills`，参见 [OpenAI 官方示例](https://developers.openai.com/cookbook/examples/codex/iterating-development-workflows-with-codex)。自定义了 `CODEX_HOME` 时，使用对应目录。

例如，在没有同名目录的情况下，可以使用 Git 下载：

```powershell
# Windows PowerShell：默认用户级目录
git clone https://github.com/sevy005/brand-strategy-proposal.git "$env:USERPROFILE\.codex\skills\brand-strategy-proposal"
```

```bash
# macOS / Linux
git clone https://github.com/sevy005/brand-strategy-proposal.git "${CODEX_HOME:-$HOME/.codex}/skills/brand-strategy-proposal"
```

也可以下载 ZIP，解压后将文件夹改名为 `brand-strategy-proposal` 再放入对应目录。已有同名 skill 时，先对比现有文件再更新。

## 调用示例

```text
请用 $brand-strategy-proposal，根据我提供的品牌资料，生成一份完整品牌策略提案。
聚焦一个主导价值，写出定位、主推产品、传播语言、视觉方向与落地计划，
并标明需要验证的关键假设。
```

```text
请用 $brand-strategy-proposal，把现有方案整理成12页提案正文。
保留已经确认的产品和定位，指出证据缺口并补充执行安排。
```

资料不完整时，可以先使用 [项目事实输入表](assets/project-intake.md)。有品牌、产品、人群或场景线索和若干可追溯事实，即可开始第一版草稿；未知信息会保留其真实状态。

## 文件结构

```text
brand-strategy-proposal/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── assets/
│   ├── project-intake.md
│   └── strategy-map.md
└── references/
    ├── strategy-formulas.md
    ├── page-blueprint.md
    ├── review-checklist.md
    └── worked-example.md
```

这是策略与提案写作 skill。PPT、PDF 或图片成品需要运行环境具备对应制作能力；参考模板中的公式不构成增长预测或经营效果承诺。
