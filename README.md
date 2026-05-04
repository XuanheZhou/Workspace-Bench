# WOLF-Bench

<div align="center">
  <img src="assets/WOLF-Bench-icon.png" alt="WOLF-Bench" width="220" />
</div>

<div align="center">
  <p><b>WOLF-Bench</b> is a benchmark for evaluating real-world agentic workflows.</p>
  <p><i>Dataset: coming soon.</i></p>
</div>

---

## 简介 / Overview

WOLF-Bench 面向 **Agent 评测**：关注模型在真实工作流中“读写文件、调用工具、多步规划与执行、产出可交付文件”的端到端能力。

WOLF-Bench focuses on end-to-end agent capability in realistic workflows:
tool use, multi-step planning/execution, file interaction, and producing deliverables.

## 框架图 / Framework

下面的框架图展示了 WOLF-Bench 的典型评测管线（任务 -> 运行 -> 统一产物 -> 评估 -> 汇总）：

```mermaid
flowchart TD
  A[Task Suite\n(Instructions + Inputs)] --> B[Runner\n(Exec Agent in Sandbox)]
  B --> C[Agent\n(LLM + Tools)]
  C --> D[Workspace\n(Files / Artifacts)]
  D --> E[Standard Outputs\n(agent.json / agent.log / output/ ...)]
  E --> F[Judge\n(Rubrics / Metrics)]
  F --> G[Leaderboard & Analysis]
  E --> H[Visualization UI]
```

## 结果 / Results

结果图与详细表格将随着论文最终版本同步更新（coming soon）。

> 结果占位图（后续替换为真实结果图）：
>
> <img src="assets/WOLF-Bench-icon.png" alt="Results (coming soon)" width="420" />

## 数据集 / Dataset

- 数据集：**coming soon**
- 我们会在发布时提供：任务说明、输入文件清单、标准化输出格式与评测脚本（如适用）。

## 引用 / Citation

如果你在研究中使用 WOLF-Bench，请引用我们的论文（arXiv 信息待补全）：

```bibtex
@misc{wolfbench2026,
  title        = {WOLF-Bench: A Benchmark for Real-World Agentic Workflows},
  author       = {TODO: Authors},
  year         = {2026},
  eprint       = {TODO: arXiv-ID},
  archivePrefix= {arXiv},
  primaryClass = {cs.CL},
  url          = {https://arxiv.org/abs/TODO}
}
```
