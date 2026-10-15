# Cilium: Up and Running · 中英对照

《Cilium: Up and Running》（Nico Vibert 等著，O'Reilly 2026）全书的**中英文段落对照**版，单文件 HTML，离线可看。

> 本仓库仅发布成品 HTML + 配图。PDF 解析、翻译分包、HTML 组装等构建脚本与中间产物在本地工作区，未一并入库。

## 目录结构

```
site/
├── Cilium-Up-and-Running-中英对照.html   ← 主文件
└── images/                                ← 89 张原书配图（HTML 相对引用）
    ├── fig_1-1.png
    ├── fig_1-2.png
    └── ...
```

## 阅读方式

**方式一：直接双击**
双击 `Cilium-Up-and-Running-中英对照.html`，用默认浏览器打开即可。所有图片走相对路径，无需联网。

**方式二：GitHub Pages（推荐）**
在仓库 **Settings → Pages** 把 Source 设为 `main` 根目录，保存后访问：

```
https://breeve.github.io/cilium-up-and-running-zh/Cilium-Up-and-Running-中英对照.html
```

**方式三：本地服务器**
想让图片/字体加载更稳，可以在仓库根目录跑：

```bash
# Python 3
python -m http.server 8000

# 或 Git Bash
npx serve .
```

然后浏览器打开 `http://localhost:8000/Cilium-Up-and-Running-中英对照.html`。

## 内容与排版

- **覆盖范围**：前言（Foreword）+ 序言（Preface）+ 第 1–16 章正文（共 2156 个段落块，索引页已排除）
- **段落对照**：英文原文在上、简体中文在下；标题三级双语；项目符号成对列表；脚注小字居段末
- **代码**：全部保留英文原文（等宽字体深色块）；行内代码与斜体标记完整还原
- **配图**：89 张原书配图从 PDF 高清裁剪嵌入，图注英文 + 中文双行
- **术语规范**：Cilium、eBPF、Pod、Service、NetworkPolicy、CRD 名、命令、版本号、URL 等保留英文；`集群 / 节点 / 工作负载 / 数据路径 / 控制平面 / 入站 / 出站 / 可观测性 / 地址伪装` 等按术语表统一

## 更新

本书首次发布于 2026-10-15，对应 O'Reilly 2026 年版（ISBN 待定）。后续若有勘误或作者更新，将重新翻译并推送 `main` 分支。

## 版权与致谢

- 原文版权归 O'Reilly Media, Inc. 与原作者所有，本仓库仅提供个人学习用途的中英文对照译稿
- 翻译与排版由 breeve 完成，欢迎提 issue 或 PR 指出错漏
- 感谢 Cilium 开源社区以及 Isovalent 团队，让 Cilium 成为 Kubernetes 网络与安全的事实标准
