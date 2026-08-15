# 汽车碰撞安全 · 被动安全性能集成工程师 Skill 包

基于《汽车碰撞安全》（[日]水野幸治 著，韩勇、陈一唯 译，人民交通出版社 2016）全书 12 章深度蒸馏生成。

## 内容

```
汽车碰撞安全-被动安全性能集成skill/
├── README.md
├── skills/
│   ├── passive-safety-integrator/SKILL.md    # 主 skill：整车被动安全性能集成（决策、权衡、红线、问题诊断）
│   ├── crashworthiness-structure/SKILL.md    # 结构耐撞性设计（吸能、波形、载荷路径、兼容性、事故再现）
│   ├── occupant-protection/SKILL.md          # 乘员保护与损伤分析（损伤准则、假人、约束系统、儿童、挥鞭伤）
│   └── pedestrian-protection/SKILL.md        # 行人保护（事故统计、损伤机理、冲击器试验、头/腿设计、自行车）
└── references/
    └── research/
        ├── 01-sources.md          # 来源清单
        ├── 02-extraction-notes.md # 结构化提取记录（含出处）
        └── 03-key-quotes.md       # 关键原文引用
```

## 使用方法

### 方式一：把文件夹放入 Codex skills 目录（推荐）

将 `skills/` 下的三个文件夹复制到 `~/.codex/skills/`：

```bash
cp -R skills/passive-safety-integrator ~/.codex/skills/
cp -R skills/crashworthiness-structure ~/.codex/skills/
cp -R skills/occupant-protection ~/.codex/skills/
cp -R skills/pedestrian-protection ~/.codex/skills/
```

重启/下一轮对话后生效，直接说"用被动安全集成工程师的方式分析…"即可触发。

### 方式二：作为参考文档使用

不安装也可以直接阅读 `SKILL.md`，作为领域知识手册与决策清单使用。

## 注意事项

- 书中的损伤准则限值、法规工况均为成书（2016）时点数据，用于正式项目前请核对现行法规原文（UN Rxx、FMVSS、C-NCAP/EuroNCAP/IIHS 最新版本）。
- 扫描版 PDF 经 OCR 提取，公式与表格数字可能有识别误差；关键数值已在提取记录中标注出处章节。
- 四份 skill 可独立使用，`passive-safety-integrator` 为总入口；`pedestrian-protection` 独立覆盖行人保护。
