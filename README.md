# PDFKit · AI 原生 PDF 处理 · PDFKit for Python

> 面向已有 .pdf 文件的处理工具箱：读取提取、自然语言编辑、格式转换、表单、加密签名、OCR

![Type](https://img.shields.io/badge/type-Agent%20Skill-4a6b7c)
![Upstream](https://img.shields.io/badge/upstream-pdfkit-py%20v1.0.1%20-%20腾讯文档%20PDFKit-8f8a80)
![License](https://img.shields.io/badge/license-归原作者-b8935a)

> ⚠️ 本仓库是个人使用环境中的 Skill 归档副本，**版权归原提供方**：pdfkit-py v1.0.1 · 腾讯文档 PDFKit

## 适用边界（先读这段）

**只处理已存在的 `.pdf` 文件。** 不处理 docx / xlsx / pptx / html / md / 图片，也不承担论文写作、文本润色、内容创作、项目管理这类任务——那些有别的 Skill 负责。

## 能力

| 类别 | 具体能力 |
|---|---|
| 读取 | 文本抽取、版面分析、表格识别、图片提取 |
| 编辑 | 基于自然语言指令的修改、页码与水印、页面增删 |
| 转换 | PDF ↔ 图片、PDF → 文本 / Markdown |
| 表单 | 表单字段读取与填写 |
| 安全 | 加密、解密、数字签名 |
| OCR | 扫描件文字识别 |
| IR | 中间表示层，用于结构化重建 |

## 环境初始化（必做）

`SKILL.md` 开头有一段强制初始化：定位 venv 中的 Python 解释器，再调用 CLI。

Windows PowerShell 必须用调用运算符，否则路径带空格会直接失败：

```powershell
& "{venv_python}" -m pdfkit <command> "<file.pdf>"
```

## 目录结构

```
pdfkit-py/
├─ SKILL.md      适用范围 · 环境初始化 · 命令参考 · 坐标系规范 · 字体
├─ scripts/      CLI 封装与批处理
└─ _icon.png
```

## 许可

该 Skill 由腾讯文档 PDFKit 提供，著作权归原提供方所有。本仓库仅为个人归档，**不作出任何再许可**，详见 `NOTICE.md`。


## 安装

```bash
git clone https://github.com/px-pangu/pdfkit-py.git ~/.workbuddy/skills/pdfkit-py
# Claude Code：~/.claude/skills/pdfkit-py
```

> 若原包依赖 CLI（如 `kdocs`、`ima`、`wecom`、`pdfkit`），需先按 `SKILL.md` 的安装与认证段落配置本机环境。**仓库内不含任何凭据。**

