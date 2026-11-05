# 莫钤麟 · 个人作品集

> 把脑子里的想法，一个一个做成能用的东西。
> 数据采集 / 自动化 / AI Agent / 桌面软件 / 网页开发 —— 全部可点开把玩。

- 在线访问：<https://dusyandu.github.io/portfolio-site/>（Pages 生效后可用）
- 开发者：莫钤麟（平顶山学院 · 2026 级）
- 联系方式：3032847459@qq.com
- GitHub：<https://github.com/dusyandu>

---

## 一、这是什么

这不是一份简历，而是一个**能跑起来的作品索引**：首页是作品卡片墙，每张卡片点进去是一页独立详情（做了啥、怎么做的、亮点在哪），再点演示区就能直接上手玩。

整个站点是纯静态的：`index.html` + `works/`，不依赖后端、不需要构建工具，双击本地文件或丢到任何静态托管（GitHub Pages / Netlify）都能跑。

站点内容由一份 JSON 数据驱动（`index.html` 里的 `DATA_START / DATA_END` 区段），改数据即可改站，不用碰页面结构。

---

## 二、作品清单（13 个）

| # | 作品 | 分类 | 核心技术 | 详情页 |
|---|---|---|---|---|
| 01 | 语音对话助手 | AI Agent | Flask · DeepSeek · edge-tts · Function Calling | [works/voice-agent.html](works/voice-agent.html) |
| 02 | 养成型桌面桌宠 | 桌面应用 | PySide6 · 状态机 · 物理回弹 · 存档 | [works/desktop-pet.html](works/desktop-pet.html) |
| 03 | 自媒体自动运营流水线 | AI Agent | Playwright · 自动化发布 · 大模型写稿 | [works/auto-media.html](works/auto-media.html) |
| 04 | 网页接口加密逆向 | 数据采集 | 两层 AES-CBC + 自实现 RSA · 纯 Python | [works/netease-crypto.html](works/netease-crypto.html) |
| 05 | GitHub 热门智能巡检 | AI Agent | 热门榜抓取 · 大模型多维打分 · 技能封装 | [works/github-patrol.html](works/github-patrol.html) |
| 06 | 本地语义记忆库 | AI Agent | ChromaDB · 中文嵌入 · 按项目隔离 | [works/local-memory.html](works/local-memory.html) |
| 07 | AI 自动玩 2048 | AI Agent | 多模态看图决策 · 感知-决策-操作闭环 | [works/ai-2048.html](works/ai-2048.html) |
| 08 | 商品价格监控雷达 | 数据采集 | 定时任务 · 整页交 AI 提取 · 走势图 | [works/price-radar.html](works/price-radar.html) |
| 09 | 智能采集框架实战 | 数据采集 | crawl4ai · AI 生成字段提取规则 · CSV | [works/crawl4ai.html](works/crawl4ai.html) |
| 10 | 网页小游戏合集 | 网页开发 | Canvas · 动效 · 操作手感打磨 | [works/web-games.html](works/web-games.html) |
| 11 | 商品评论批量采集 | 数据采集 | 展开折叠区 · 模拟滚动触发懒加载 · 去重落盘 | [works/comment-collector.html](works/comment-collector.html) |
| 12 | 计划管理后端 | 网页开发 | Flask · SQLAlchemy · SQLite · 跨域 | [works/plan-backend.html](works/plan-backend.html) |
| 13 | 工具打包集 | 桌面应用 | PyInstaller · 单文件 / 带素材 / 三方库 / 多模块 | [works/pack-toolkit.html](works/pack-toolkit.html) |

分类分布：AI Agent 5 个 · 数据采集 4 个 · 桌面应用 2 个 · 网页开发 2 个。

### 作品主线怎么串起来的

- **采集 → 结构化 → 可视化**：爬回来、洗干净、落成 CSV / 图表（08·09·11）。
- **采集 → 交给模型判断**：不写死规则，让 AI 读整页内容做提取或打分（05·08·09）。
- **模型 → 动手操作**：感知屏幕、决策、执行，形成闭环（07·03）。
- **模型 → 长期记忆**：把偏好和踩过的坑存进本地向量库，跨会话复用（06）。
- **工程收口**：后端接口（12）、桌面封装（02）、打包成 exe（13）——把脚本变成别人能用的东西。

---

## 三、成长轨迹（5 站）

| 阶段 | 主题 | 关键节点 |
|---|---|---|
| 1 | 起步 · 把数据抓回来 | Requests 静态抓取 → DrissionPage 浏览器自动化 → 列表页/详情页规则提取 |
| 2 | 深入 · 跟加密和反爬过招 | AES + RSA 接口逆向 → crawl4ai 由 AI 生成提取规则 → CSV/Excel 落盘 |
| 3 | 进阶 · 让数据动起来 | Flask 接口 → SQLAlchemy 读写 SQLite → 数据可视化 |
| 4 | 打磨 · 做成能用的软件 | PySide6 桌面应用 → PyInstaller 打包 → 状态机与交互动效 |
| 5 | 当前 · 让 AI 自己干活 | Function Calling 工具调用 → 向量检索记忆 → 浏览器自动化运营 |

---

## 四、技能自评

不吹精通，只标熟练度（5 分制，全部点亮≈敢拿它交付项目）。

| 技能 | 分值 | 技能 | 分值 |
|---|---|---|---|
| Python | 5 | HTML / CSS / JS | 4 |
| 数据采集 / 清洗 | 4 | PySide6 桌面应用 | 3 |
| Requests / DrissionPage | 4 | PyInstaller 打包 | 4 |
| Flask / 接口开发 | 4 | 大模型 API / 工具调用 | 4 |
| SQLAlchemy / SQLite | 3 | 向量检索 / RAG | 3 |
| 浏览器自动化 | 4 | 加密逆向分析 | 3 |

---

## 五、目录结构

```
portfolio-site/
├── index.html            # 首页：作品卡片墙 + 成长轨迹 + 技能 + 关于 + 联系
├── admin.html            # 可视化后台：改文字/加作品，实时预览，一键导出整站
├── .nojekyll             # 让 GitHub Pages 跳过 Jekyll 处理，别删、别改名
├── README.md             # 本文
└── works/
    ├── *.html            # 13 个作品详情页
    ├── assets/pet/       # 桌宠表情素材
    └── demo/             # 各作品的在线演示（含 voice/ 子目录）
```

演示页和详情页是两套东西：详情页讲「怎么做的」，演示页是「动手试」。详情页里的演示区用 iframe 直接内嵌演示页。

---

## 六、本地预览

纯静态，不需要装任何环境：

1. 直接双击 `index.html`；
2. 或起一个本地服务（更接近线上环境）：`python -m http.server 8000`，再打开 <http://127.0.0.1:8000>。

---

## 七、部署到 GitHub Pages

仓库已就绪，Pages 只需开一次开关：

1. 打开 `Settings` → 左侧 `Pages`
2. Source 选 `Deploy from a branch`，Branch 选 `main`，目录选 `/(root)`
3. 点 `Save`，等 1~2 分钟，访问 <https://dusyandu.github.io/portfolio-site/>

以后更新内容只需：

```bash
git add . && git commit -m "update content" && git push
```

浏览器记得 `Ctrl + F5` 强刷。

---

## 八、以后改内容（不用碰代码）

打开站点地址后加 `/admin.html`，在左边表单里改文字、加作品，右边实时预览，点「⚡ 生成完整站点」导出新包，再把 `index.html` 和 `works/` 覆盖回仓库即可。

---

## 免责声明

本项目中的网页数据采集、接口加密分析、浏览器自动化等内容，**仅供学习交流与技术研究**，请勿用于任何商业用途或侵犯他人权益的用途。抓取时应遵守目标站点的 robots 协议与相关法律法规，控制请求频率。
