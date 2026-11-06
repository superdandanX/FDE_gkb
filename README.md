# 青禾优选 W01 作业提交

- 产品版本：`0.2.0-w1`
- 能力矩阵：`w1-capabilities-0.2.0`
- fit-gap 契约：`w01-0.2.1`
- 模型：`deepseek-chat`（Chat Completions，`deepseek-low` 配置）

## 内容

- `artifacts/w01/`
  - `environment_check.json`：9 项环境检查
  - `model_baseline.json`：真实模型与 9 次场景运行
  - `runtime_evidence.json`：11 个行为场景与证据哈希
  - `product_fit_gap.json` / `product_fit_gap.xlsx`：6 条初步适配判断
  - `promptfoo-results.json`：7 个评估用例的原始结果
  - `evidence/`：11 份场景记录与 `trace.jsonl`
- `docs/w01/`
  - `project_assessment.md`：立项分析报告
  - `interview-1.md`：沈总访谈记录
  - `interview-transcript.json`：访谈原始导出

## 说明

- `artifacts/` 中的 JSON 与 `evidence/` 均由实际运行生成，未手工修改；产品行为验证 11/11，Promptfoo 7/7。
- fit-gap 为 W01 初步版，共 6 条（GAP-001～006）；客户说法均按“角色转述/未知”标注，未写成已核实。
- 未包含 `.venv`、`.runtime`、`node_modules`、密钥或未改动的工程文件。
- 可用官方工程运行 `tools/check_product.py --root <本目录>` 复核结构。
