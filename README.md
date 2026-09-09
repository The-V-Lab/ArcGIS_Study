# ArcGIS Study | ArcGIS 系统入门

一套面向 GIS 初学者的中英文 ArcGIS 系统学习项目，从空间思维、数据模型与坐标系出发，逐步覆盖 ArcGIS Pro 项目管理、地图表达、查询与连接、基础地理处理、编辑、布局输出、ArcGIS Online 分享、可重复工作流和责任边界。

> **English summary:** A bilingual, beginner-friendly ArcGIS learning module covering spatial thinking, data models, coordinate systems, ArcGIS Pro workflows, cartography, geoprocessing, ArcGIS Online sharing, reproducibility, quality assurance, and responsible spatial practice.

## 课程入口

| 语言 | R Markdown 源文件 | 已生成 HTML |
|---|---|---|
| 中文 | [arcgis_getting_started.Rmd](./arcgis_getting_started.Rmd) | [arcgis_getting_started.html](./arcgis_getting_started.html) |
| English | [arcgis_getting_started_en.Rmd](./arcgis_getting_started_en.Rmd) | [arcgis_getting_started_en.html](./arcgis_getting_started_en.html) |

HTML 文件为自包含页面，可在克隆或下载仓库后直接使用浏览器打开。GitHub 的普通文件预览不会把 HTML 当成课程网站运行。两份页面顶部提供中英文切换；若复制到其他位置，请将两个 HTML 放在同一目录中。

## 项目目标

本项目不把 ArcGIS 教成一组需要记忆的按钮，而是建立一条可以检查、解释和重复的空间分析链：

> **提出空间问题 → 检查数据与元数据 → 选择坐标系 → 浏览与制图 → 查询、连接与分析 → 验证输出 → 设计地图 → 安全分享**

完成课程后，学习者应能够：

- 解释空间数据的几何、属性、空间参考和元数据；
- 区分项目、地图、图层、数据集、布局、项目项、Web 图层和 Web 地图；
- 认识点、线、面、栅格和非空间表的适用场景；
- 在 ArcGIS Pro 中创建项目、连接数据、检查属性并组织输出；
- 区分地理坐标系与投影坐标系，以及 **Define Projection** 与 **Project**；
- 根据变量类型选择符号、颜色、分类、标签和弹窗；
- 正确使用属性查询、空间选择、属性连接和空间连接；
- 理解 Buffer、Clip、Dissolve、Intersect、Spatial Join、Near 等基础工具；
- 进行记录数、字段、范围、单位、几何与边界案例检查；
- 创建布局、导出地图，并在 ArcGIS Online 中按目标受众分享；
- 使用 Geoprocessing History、ModelBuilder 和 ArcPy 开始构建可重复流程；
- 识别隐私、误导性制图、生态谬误、MAUP 和空间相关等风险。

## 适用对象

- 第一次系统学习 GIS 或 ArcGIS 的学生；
- 需要将地图和空间分析用于研究的人员；
- 公共卫生、环境、城市规划、商业分析及公共管理学习者；
- 希望从“会操作软件”进阶到“能解释和验证工作流”的 ArcGIS 用户。

课程预计学习时间约为 **150–210 分钟**，可按章节分次完成。仅要求基本的文件和表格操作能力，不要求 R、Python 或 GIS 基础。

## 软件范围

课程以 **ArcGIS Pro 3.x** 为桌面主线，并介绍 ArcGIS Online 的 Web 地图和内容分享流程。

- ArcGIS Pro 用于本地数据管理、制图、编辑、空间分析和布局；
- ArcGIS Online 用于内容管理、托管图层、Web 地图、弹窗和分享；
- ArcGIS Enterprise、Field Maps、Survey123、Dashboards、StoryMaps 等作为生态扩展介绍；
- ModelBuilder、ArcPy 和 Arcade 作为自动化与表达式工具入门。

ArcGIS Pro 运行于 Windows。macOS 或 Linux 学习者可以阅读全部内容，并通过组织提供的远程 Windows、虚拟机或 ArcGIS Online 完成适用部分。具体工具、扩展、用户类型、credits 和分享权限取决于 ArcGIS 版本及组织配置。

## 课程结构

| 模块 | 核心内容 |
|---|---|
| 1. GIS 与 ArcGIS 全景 | GIS 问题类型、ArcGIS Pro、Online、Enterprise 与应用生态 |
| 2. ArcGIS Pro 项目与界面 | `.aprx`、默认 geodatabase、toolbox、Contents、Catalog 和 Geoprocessing |
| 3. 空间数据基本模型 | 点、线、面、栅格、表、feature class、layer 和常见格式 |
| 4. 坐标系与投影 | GCS、PCS、datum、动态投影、Define Projection 与 Project |
| 5. 添加与检查数据 | 文件夹、geodatabase、Portal、CSV 转点、元数据与到货 QA |
| 6. 地图浏览与表达 | 符号化、归一化、分类、颜色、标注、弹窗和比例尺 |
| 7. 查询与地理处理 | 属性/空间选择、join、Buffer、Clip、Dissolve、Intersect 和 Near |
| 8. 完整实践 | 虚构社区公共服务 1 km 覆盖缺口分析 |
| 9. 编辑与完整性 | snapping、domain、subtype、topology 和安全编辑 |
| 10. 布局与导出 | Map Frame、标题、图例、来源、PDF/PNG 和地图 QA |
| 11. ArcGIS Online | hosted feature layer、view、web map、权限和依赖检查 |
| 12. 可重复工作流 | History、ModelBuilder、ArcPy、Arcade、日志与命名 |
| 13. 故障排查 | 数据源、坐标系、选择、环境、锁、join、许可和 Web 权限 |
| 14. 责任与空间推断 | 隐私、聚合、生态谬误、MAUP、分类和因果边界 |
| 15. 练习与快速参考 | 概念题、综合项目、术语表、工具卡和最终检查清单 |

## 贯穿教学案例

课程使用一个完全虚构的“社区公共服务覆盖”案例：

- 社区以面要素表示，并带有人口等属性；
- 服务设施以点要素表示；
- 使用适合研究区且以米为单位的投影；
- 为设施创建 1 km 缓冲区；
- 使用社区中心点与 Spatial Join 初筛潜在覆盖缺口；
- 对输入/输出计数、坐标系、单位、边界案例和工具消息进行验证；
- 将结果制作成地图并讨论分享权限与隐私。

R Markdown 使用固定随机种子 `20260908` 生成示意社区、设施、距离和人口，因此中英文页面得到一致、可重复的教学图和结果表。

该案例只解释**直线距离缓冲**。它没有模拟道路、障碍、入口、坡度、出行方式、营业时间、容量或费用，因此不能替代网络可达性分析或真实选址决策。

## 项目特点

- **中英对照：**两份课程保持相同章节、案例、代码、表格、练习和警示结构；
- **完整学习路径：**从概念、操作到验证、交付与责任边界；
- **可重复示意：**使用 base R 生成固定教学数据和原创示意图；
- **无需 ArcGIS 即可阅读：**HTML 可离线打开，ArcPy 示例不会在构建时执行；
- **自包含 HTML：**CSS、JavaScript 和教学图均嵌入最终页面；
- **响应式设计：**支持桌面、手机和打印布局；
- **无障碍考虑：**语义化导航、替代文本、键盘焦点、高对比色和减少动画设置；
- **双向语言导航：**中文与英文页面可直接互相切换；
- **质量控制导向：**每个工作流都强调数量、字段、坐标、单位和边界案例验证；
- **责任边界明确：**包含公开分享、敏感位置、数据许可与空间推断限制。

## 文件结构

```text
ArcGIS_Study/
├── README.md
├── arcgis_getting_started.Rmd
├── arcgis_getting_started.html
├── arcgis_getting_started_en.Rmd
├── arcgis_getting_started_en.html
├── styles.css
└── includes/
    └── vlab-brand.html
```

| 文件 | 作用 |
|---|---|
| `README.md` | 项目介绍、使用方式、构建与维护说明 |
| `arcgis_getting_started.Rmd` | 中文课程源文件 |
| `arcgis_getting_started.html` | 中文自包含课程页面 |
| `arcgis_getting_started_en.Rmd` | 英文课程源文件 |
| `arcgis_getting_started_en.html` | 英文自包含课程页面 |
| `styles.css` | 页面颜色、布局、提示框、表格、响应式和打印样式 |
| `includes/vlab-brand.html` | 页面顶部 The V Lab · ArcGIS 品牌组件 |

## 快速开始

### 1. 克隆仓库

```bash
git clone https://github.com/LaboratoireV/ArcGIS_Study.git
cd ArcGIS_Study
```

也可以使用 GitHub 的 **Code → Download ZIP**，解压后进入项目目录。

### 2. 打开课程

无需安装 R 或 ArcGIS，直接在本地浏览器打开：

- `arcgis_getting_started.html`：中文；
- `arcgis_getting_started_en.html`：English。

页面中的外部官方资源链接需要网络连接，其余主体内容、样式和示意图均包含在 HTML 中。

### 3. 完成操作练习

若要在 ArcGIS Pro 中复现操作：

1. 使用组织账号或获授权的 ArcGIS Pro 环境；
2. 根据本地研究区选择合适的真实数据和坐标系；
3. 不要将教程中的占位 WKID `00000` 直接用于 ArcPy；
4. 按教程记录参数、环境设置、工具消息和验证结果；
5. 发布 Web 内容前核查角色、credits、编辑权限、隐私和数据许可。

## 从 R Markdown 重新生成 HTML

### 环境要求

- R；
- `rmarkdown`；
- `knitr`；
- Pandoc（RStudio 通常自带）。

课程的教学图和表只依赖 base R 与 `knitr`，不要求 `sf`、`terra`、ArcPy 或 ArcGIS 安装。

### 安装 R 包

```r
install.packages(c("rmarkdown", "knitr"))
```

### 使用 RStudio

1. 在 RStudio 中打开任一 `.Rmd`；
2. 确保 `styles.css` 与 `includes/vlab-brand.html` 保持当前相对路径；
3. 点击 **Knit → Knit to HTML**；
4. 检查生成页面中的目录、语言链接、示意图、表格和折叠代码。

### 使用命令行

生成中文版：

```bash
Rscript -e 'rmarkdown::render("arcgis_getting_started.Rmd")'
```

生成英文版：

```bash
Rscript -e 'rmarkdown::render("arcgis_getting_started_en.Rmd")'
```

同时生成：

```bash
Rscript -e 'for (f in c("arcgis_getting_started.Rmd", "arcgis_getting_started_en.Rmd")) rmarkdown::render(f, envir = new.env(parent = globalenv()))'
```

当前成品已在以下环境中完成验证：R 4.6.1、knitr 1.51、rmarkdown 2.31 和 Pandoc 3.8.3。其他较新的兼容版本通常也可使用；构建失败时应先运行 `rmarkdown::pandoc_available()` 检查 Pandoc。

输出采用：

- `html_document`；
- 自包含资源；
- Flatly 主题与 Tango 代码高亮；
- 三级浮动目录和章节编号；
- 可折叠代码；
- MathML 数学表达；
- 响应式、手机和打印样式。

## 修改与维护

### 保持中英文一致

课程正文应优先修改 `.Rmd` 源文件，再重新生成对应 HTML；不要只修改生成后的 HTML。修改课程时，应同步检查：

- 标题、章节顺序与学习目标；
- 贯穿案例的数据生成代码和随机种子；
- 表格、工具参数、练习和折叠答案；
- 图注、替代文本和提示框；
- 两个页面之间的语言链接；
- 官方文档 URL、ArcGIS 版本描述和权限说明。

### 修改文件名

如果更改 HTML 文件名，必须同步修改：

- 两个 Rmd 中 `.language-switch` 的链接；
- `includes/vlab-brand.html` 的首页链接；
- README 中的课程入口和文件结构。

### 发布前检查

1. 两份 Rmd 都能无错误渲染；
2. 中英文页面章节与教学结果一致；
3. HTML 在桌面和窄屏视口没有页面级横向滚动；
4. 目录、语言切换和折叠答案可正常使用；
5. 图片完整加载并包含替代文本；
6. 浏览器控制台没有错误；
7. 最终 HTML 不依赖本地绝对路径；
8. 敏感数据、凭据、访问令牌和个人信息未进入仓库。

## 数据、代码与责任边界

- 本仓库是教学文档项目，不包含 `.aprx`、`.gdb`、`.atbx`、真实 GIS 数据或可直接运行的 ArcGIS Pro 工程；
- 所有社区、设施、距离和人口均为固定种子生成的教学示意，不对应真实地点或个人；
- 教程中的 ArcPy 代码仅说明工作流结构，需要在 ArcGIS Pro Python 环境中补充真实路径、坐标系、许可和错误处理；
- 教程不能替代当地空间数据标准、隐私审查、专业网络分析或业务决策；
- 直线缓冲、空间重叠和视觉聚集不自动证明真实可达性或因果关系；
- 使用外部数据时，应核查来源、时间、比例尺、精度、许可、署名和再分享条件；
- 公开 hosted feature layer 或 Web map 前，应按最小权限原则检查其所有依赖图层。

## 许可说明

本仓库当前未包含 `LICENSE` 文件，因此没有声明通用的开源复用许可。需要复制、改编或再发布仓库内容时，请先联系仓库维护者并同时遵守 Esri、底图及外部数据各自的许可与署名要求。

## 官方学习资源

- [ArcGIS Pro Documentation](https://pro.arcgis.com/)
- [ArcGIS Pro Quick-start Tutorials](https://pro.arcgis.com/en/pro-app/latest/get-started/pro-quickstart-tutorials.htm)
- [What is geoprocessing?](https://pro.arcgis.com/en/pro-app/latest/help/analysis/geoprocessing/basics/what-is-geoprocessing-.htm)
- [Introduction to the geodatabase](https://pro.arcgis.com/en/pro-app/latest/help/data/geodatabases/overview/what-is-a-geodatabase-.htm)
- [Coordinate systems, projections, and transformations](https://pro.arcgis.com/en/pro-app/latest/help/mapping/properties/coordinate-systems-and-projections.htm)
- [What is ArcPy?](https://pro.arcgis.com/en/pro-app/latest/arcpy/get-started/what-is-arcpy-.htm)
- [Get started with data in ArcGIS Online](https://doc.arcgis.com/en/arcgis-online/get-started/get-started-with-data.htm)
- [Get started creating maps in ArcGIS Online](https://doc.arcgis.com/en/arcgis-online/reference/get-started-with-maps.htm)
- [Get started with sharing in ArcGIS Online](https://doc.arcgis.com/en/arcgis-online/get-started/get-started-with-sharing.htm)

## English overview

**ArcGIS Study** is a bilingual introductory course designed for learners with no prior GIS experience. It connects conceptual understanding with an auditable workflow: define a spatial question, inspect data and metadata, choose an appropriate coordinate system, create a map, run basic queries and geoprocessing tools, validate outputs, communicate limitations, and share content responsibly.

The English module mirrors the Chinese module section by section and includes the same fixed-seed fictional community-service-access example. The prebuilt HTML is self-contained and can be read without R, Python, ArcGIS, or an ArcGIS account. Hands-on ArcGIS Pro and ArcGIS Online exercises still require the relevant software, organizational privileges, licences, and—in some workflows—credits or extensions.

This is an independent learning module rather than official Esri training. Product interfaces and privileges change over time; consult the official documentation that matches your installed version and organization.

---

Maintained as part of **The V Lab** bilingual learning modules.
