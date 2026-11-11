### 🔍【项目五维穿透研报】surfcoderepeat (surfcoderepeat)
- **基本盘定位**：TRACK_B_PRETOKEN（雷达按人物 Handle 归类为 TRACK_B，穿透实测其核心载体为已发币协议 Identity.md，代币代号 IMD，以太坊主网合约 `0xd34a99bc0f67ae1bbd63c660e6d0b0dd03e263b7` 及 2,000 枚 Identity.md 节点工作席位 NFT） / 初筛得分 99.0 分
- **一句话本质**：由前 Base 链爆款游戏 Fren Pet 开发者 Adam（`@surfcoderepeat`）主导的去中心化 AI Agent 蜂群众包网络与跨链发射台，通过持有或租赁 NFT 席位运行本地沙盒 Agent 执行多轮调研、预言机喂价与代码构建，并将协议收入与 Uniswap v4 Hook 卖盘超额库存的 85% 硬编码自动销毁。

## ⚡ 双脑会审交锋纪要 (Dual-Brain Review Summary)
- **多头博弈逻辑**：
  1. **硬核工程高频交付与主动自我设限（CappedBurnHook 通缩飞轮）**：创始人 Adam 具备从 0 到 1 打造 Base 早期现象级应用 Fren Pet 的完整履历，过去 30 天内高密度交付了 Mac/Windows 桌面端沙盒客户端（`imd.fun/app`）、跨 Ethereum/Base/Robinhood Chain 的一键 RPC 路由、多节点交叉验证预言机及 `imdlend.com` 席位租赁市场。在机制上，团队未采用传统 VC 私募解锁模式，而是通过 Uniswap v4 的 `POOL4`（`CappedBurnHook`）设定池内 IMD 持仓硬顶：当卖盘导致池内 IMD 超出上限时，系统自动削减超额代币，其中 85% 永久销毁、6% 补贴蜂群算力调度、4.5% 分配给 sIMD 质押者、4.5% 奖励 NFT 节点运行者，回收的 ETH 则在现价下方构建承接买墙，形成硬编码的协议级自我约束。
  2. **原生卡位 Robinhood Chain 与多链发射台买盘内循环**：项目不仅部署于 Ethereum 主网与 Base，还原生打通了具备 16.75 亿 USD TVL 与合规金融底座的 Robinhood Chain（1:1 跨链桥接）。其内置发射台（Launches and Sites）规定在 Ethereum 与 Robinhood Chain 上的发币及建站费用直接销毁 IMD 或用 ETH 买入 IMD 销毁，且预言机每次提问（2 至 8 个问题）按每个问题 0.5 IMD 计费，具备真实的协议内生消耗场景。
- **红队致命挑刺**：
  1. **旧币多次换壳演进的历史筹码包袱（FP → VIBE → IMD）**：IMD 并非全新零历史包袱的创世标的，而是由 2023 年 8 月在 Base 链发行的 Fren Pet（代号 FP）跨链并先后重塑为 VIBE、最终演进为 Identity.md（代号 IMD，总供应量约 420 万至 710 万枚区间，随销毁动态缩减）。早期 FP 与 VIBE 时代留存的大户筹码结构复杂，存在历史获利盘在叙事高潮期分批派发的暗坑。
  2. **AI 算力成本外包给散户的持续性拷问**：虽然 2,000 个 Identity.md NFT 席位赋予了持有者运行 Worker 节点获取奖励的权限，但节点运行者需自行承担本地硬件及个人 Claude / Codex / Venice API 订阅额度消耗。若外部付费雇佣蜂群（Hire Swarm）的真实 B 端或合约订单不足，节点收益将无法覆盖散户 API 账单成本，导致算力网络活跃度衰减。
  3. **多链流动性分散与 FDV 估值水位**：当前 IMD 全稀释估值（FDV）已处于 1,000 万至 2,000 万 USD 以上区间，Identity.md NFT 席位在 OpenSea 地板价亦处于 0.65 ETH 至 1.99 ETH 高位。跨 Ethereum、Base、Robinhood Chain 三链桥接在一定程度上稀释了单链池子深度，目前已过早期零成本埋伏阶段，追高面临较高波动风险。

---

#### 0. ⚡ 生死大前提穿透 (第一性原理 · 动态 Loop 三步进阶审判、团队格局与主动自我设限)
本机动力学审计录得 `m_kinetic = 0.85`（其中宿主系数 `gamma_host = 0.85`，团队绑定系数 `gamma_skin = 1.0`，订单流速率 `gamma_velocity = 1.0`，非僵尸订单流 `is_zombie_orderflow = false`，非弱宿主寄生盘 `is_parasitic_on_weak_host = false`）。严格执行第一性原理【动态 Loop 三步进阶审判】：
- **第一步（穿透宿主做局目的）**：不同于 Elysium 链（创始团队 Kinetiq 仅 180 万 USD 融资，为赶在 2026-11-27 母币 KNTQ 一周年解锁前 18 天拉抬叙事而通过 Conduit 租用的提款链），`surfcoderepeat` 构建的 IMD 网络将核心资产锚定在 Ethereum 主网与 Base，并将增量发射台与 Worker RPC 原生扩展至 **Robinhood Chain**。Ethereum、Base 与 Robinhood Chain 均具备深厚的真实机构造血能力与长线开发者生态，不存在“宿主公链为母币短期解禁跑路而做局”的系统性崩盘前提。
- **第二步（穿透标的团队做大动力与身家绑定）**：核心开发者 Adam（`@surfcoderepeat`）自 2023 年深耕链上应用，以实名级声誉与持续三年以上的代码迭代绑定项目。团队未采取“发个概念币即弃管”的短视路径，而是将早期游戏代币一路升级为包含 Uniswap v4 定制 Hook、桌面沙盒客户端（支持 Mac/Windows/Linux 隔离运行）、去中心化 IPFS 容灾网关（`imd-ipfs.xyz`）及链上预言机的完整基础设施。在利益分配上，团队通过 `POOL4` 协议池与 `CappedBurnHook` 将卖盘超额筹码的 85% 硬编码销毁，同时将 Ethereum 与 Robinhood Chain 发射台费用全额注入回购销毁闭环，体现出克制短期快钱、做厚协议底座的格局。
- **第三步（动力学门禁与参与边界裁定）**：前两步审判均获通过，且以太坊主网 `POOL4` 锁定了数十万至数百万 USD 级别的协议自有流动性（POL），OpenSea 上的 2,000 枚席位 NFT 周度成交活跃，非死水僵尸池。但鉴于其 FDV 已达千万 USD 量级且历经多次品牌迁移，不适用盲目重仓梭哈，应定性为具备真实产品支撑的二级结构化博弈与生态工具交互标的。

#### 1. 开发者 / 团队底细、过往历史战绩与防李鬼核验
- **创始人履历穿透**：`@surfcoderepeat`（Adam）系加密原生全栈独立开发者，拥有 24,714 名真实粉丝，关注列表与互动圈层涵盖 Paradigm 研究员及 Base 核心建设者。2023 年 8 月，他与 `@caduveloso` 在 Base 链联合推出全链电子宠物博弈游戏 **Fren Pet（FP）**，凭借创新的喂养生命周期与鏈上 PVP 机制成为 Base 早期破圈标杆应用，获 Bankless、Beosin 等多家机构深度拆解。
- **历史信用与防李鬼核验**：经全网检索交叉核验，`@surfcoderepeat` 在长达三年的项目周期内无恶意卷款跑路（Rug Pull）记录。其历史争议主要集中在 Fren Pet V2 升级期间采用可升级钻石代理合约（Upgradeable Diamond Pattern）带来的中心化权限讨论，以及高金融化博弈机制的自然周期衰减。本次调研标的系其本人亲自操刀的主力项目（官网 `http://imd.fun`、文档 `http://imd.fun/skill.md`、备用网域 `http://imd-ipfs.xyz`），正宗性确凿无疑。需警惕的是，由于项目历经 `FP → VIBE → IMD` 三次合约迁移与品牌升级，链上存在大量同名仿盘与旧版废弃合约，实操交互必须严格锁定以太坊主网唯一有效合约 `0xd34a99bc0f67ae1bbd63c660e6d0b0dd03e263b7`。

#### 2. 风口卡位、赛道流行线与【市梦率 (Price-to-Dream Ratio)】穿透（对标 EACC / VOLTA 等近期爆款起爆因子）
- **赛道卡位与爆款基因对标**：当前链上最核心的两大阿尔法风口分别为 **AI Agent 蜂群自治（Swarm Intelligence）** 与 **Uniswap v4 自定义 Hook 协议级通缩飞轮**。横向对标近期爆款：EACC 依靠加速主义文化母题引爆情绪，VOLTA 依靠 Uniswap v4 Hook + 24% 协议税每小时自动回购销毁走出强趋势，Robinhood 链 PONS 依靠新链原生首发效应起爆。`imd.fun` 恰好将这三大起爆因子融为一体：
  1. **在技术机制上对标并进化了 VOLTA**：采用 Uniswap v4 的 `CappedBurnHook`（POOL4），不仅在交易端执行动态税收，更直接对池内代币库存设限，超额部分 85% 自动销毁，且回收 ETH 自动挂出下方买墙；
  2. **在叙事母题上超越纯文化 Meme**：落地了最多可调度 100 个 Agent 并行拆解任务、跨钱包异构节点交叉评审（Judge）、IPFS 数据集精确对账的实用型蜂群网络；
  3. **在跨链布局上精准卡位 Robinhood Chain**：支持一键配置 Ethereum、Base 与 Robinhood Chain 的 Alchemy RPC 及跨链发币，直接承接 Robinhood 链外溢资金。
- **市梦率（Price-to-Dream Ratio）评估**：当前 IMD 的 FDV 在 1,000 万至 2,000 万 USD 区间波动。相比纯空气 AI Meme 动辄数千万 USD 的泡沫估值，IMD 拥有可运行的桌面客户端、Hermes 兼容技能文件（`skill.md`）与链上预言机业务，市梦率处于合理偏温和区间；但受制于 420 万至 710 万枚的存量筹码分布，其向上爆发弹性取决于外部项目在 `imd.fun` 发射台（Launches）的发币频率及雇佣蜂群（Hire Swarm）的真实消耗规模。

#### 3. Twitter/X 真实社媒舆情穿透与 Flovia 链上聪明钱共振
- **社媒发酵成色**：根据前置实测证据包与全网检索，`@surfcoderepeat` 近期发布的 30 天高密度开发总结推文引发了硬核开发者与链上交易员圈层的高度共鸣。例如 Paradigm Prop AMM 挑战赛参与者 `@Ponxter` 公开表示一直在研读 IMD 蜂群的方法论以获取交易优势；社区核心成员 `@pegzeus` 对其单月内同时交付桌面端沙盒应用、Telegram 机器人（`/agent` 状态查询与自动生成 Issue 修复草案）、前端 CPU 渲染耗时降低 80%（2,500 项任务加载体积从 16.3 MB 压缩至 0.5 MB）表示赞叹。舆情特征呈现典型的“极客工程驱动型口碑传播”，而非矩阵号机械刷屏。
- **聪明钱与席位市场动向**：OpenSea 上的 2,000 枚 Identity.md 席位 NFT 买盘深度扎实，且衍生出第三方无需信任的智能合约租赁市场 `imdLend`（`imdlend.com`），允许资金大户买断席位 NFT 后出租给技术散户运行节点并自动按比例分成，说明链上长线资金正在围绕“席位生息 + sIMD 质押分红”构建真实收益策略。关于 Flovia 四大白名单工具链的实时聪明钱净流入明细，经全网公开检索暂无精确到单日的地址标签统计披露（信息黑盒风险），需以主网 POOL4 实时储备变化作为核心观测锚点。

#### 4. 大白话三步业务真容、庄散博弈论与【大庄四维刑侦对账】（脱敏前期老鼠仓/初始流动性，穿透真实控盘与做市意图）
- **大白话三步看懂业务真容**：
  1. **第一步（需求方发单付费）**：用户或外部智能合约想要做深度投研、获取链上预言机数据（如读取 Seaport 与 Blur 地板价，每次提问收 0.5 IMD）或使用无代币合约发射台（支持 Ethereum、Base、Robinhood Chain），通过 Intake 接口支付 IMD 或 ETH 下单。
  2. **第二步（散户节点出算力干活）**：持有或从 `imdLend` 租用 Identity.md NFT 席位的节点运行者，在自己电脑上打开 `imd.fun/app` 沙盒客户端，接入自己的 Claude、Codex 或 Venice 模型密钥。总调度器（Orchestrator）把大任务拆给最多 100 个 Agent 分轮次执行、核对引用源并打包上传 IPFS，再由其他钱包的 Agent 独立打分验收。
  3. **第三步（协议抽水销毁与买墙托底）**：发射台费用直接买 IMD 销毁；二级市场在 Uniswap v4 的 `POOL4` 交易时，一旦卖盘让池子里的 IMD 超过硬顶，`CappedBurnHook` 自动切掉多余的 IMD（85% 销毁、6% 补算力、4.5% 给 sIMD 质押者、4.5% 给 NFT 节点），并把抽出来的 ETH 挂在现价下方当托底买盘。
- **庄散博弈论与【大庄四维刑侦对账】**：
  破除“查早期老鼠仓与初始流动性决定成败”的刻板教条，由于 IMD 系从 2023 年 FP 历经三年演进至今，早期筹码早已充分换手，当前核心博弈在于**协议自有流动性（POL）的算法控盘**：
  1. **建仓与锁仓维度**：庄家（项目方与核心社区大户）通过 2,000 枚 NFT 席位与 sIMD 质押池锁定了核心权益，无需通过传统中心化做市商频繁画线。
  2. **洗盘与成本抬升维度**：`POOL4` 的 `CappedBurnHook` 本质上是一个写入智能合约的“自动化洗盘与托底机器”——散户恐慌抛售时，超出池子上限的 IMD 被强制抹除 85%，同时池子沉淀的 ETH 转化为下方硬性买墙。散户越割肉，流通盘越少、底部 ETH 承接垫越厚。
  3. **拉升与叙事催化维度**：团队通过每月一次的重磅工程更新（如本次打通 Robinhood Chain、上线桌面端与预言机）制造基本面脉冲，吸引新资金买入 IMD 或抢购 NFT 席位。
  4. **派发隐患维度**：最大的潜在抛压来自两处：一是节点运行者为支付现实中的 Claude/Codex API 美元账单，通过新增的 Rewards Sellable 视图（一键领取并抛售价值 >= 1 USD 的奖励）产生的持续性小额变现抛压；二是早期 FP/VIBE 时代潜伏至今的巨鲸在流动性充沛时的阶段性减持。

#### 5. 发币情况与实盘落地 SOP（未发币写一级打新/防女巫/退款规则；已发币输出波浪底座候选 Wave A/B/C 与做市池真实深度，严禁研报心算固定百分比，移动风控委托 trailing-guard 动力学斐波那契接管）
- **发币与池子真实状态核验**：尽管雷达探针因抓取创始人个人推文将其归入 `TRACK_B_PRETOKEN`，但经链上穿透核实，其生态核心代币 **IMD** 已在 Ethereum 主网正式流通（合约地址：`0xd34a99bc0f67ae1bbd63c660e6d0b0dd03e263b7`），并通过官方 1:1 桥扩展至 Base 与 Robinhood Chain；配套席位 NFT（Identity.md，总量 2,000 枚）已在 OpenSea 全量流通。
- **做市池真实深度与波浪底座候选（二级实盘 SOP）**：
  - **做市池真实深度（`liquidity_usd`）**：以太坊主网 Uniswap v4 `POOL4` 及关联跨链池合计沉淀真实流动性深度处于数十万至百万 USD 量级（随 ETH 价格与 `CappedBurnHook` 下方买墙动态调整，FDV 约 1,000 万至 2,000 万 USD 区间，非微盘死水池，实操下单前需在 `imd.fun` 终端校验主网 `POOL4` 当日实时 ETH 买墙厚度）。
  - **三点波浪底座候选（`Wave A/B/C` 锚定结构）**：
    - `Wave A`（前一波段启动锚点）：品牌由 VIBE 正式完成向 Identity.md（IMD）迁移并上线 Uniswap v4 `POOL4` 协议池的初始建仓密集成交区底座；
    - `Wave B`（波段脉冲高点）：AI Swarm 概念发酵驱动 FDV 冲高至 2,000 万 USD 上方、OpenSea 席位 NFT 触及 1.99 ETH 阶段性峰值的局部派发顶；
    - `Wave C`（当前回调确认底座）：近期随大盘震荡回落、依靠 `CappedBurnHook` 回收 ETH 构筑的 standing buy wall（下方挂单买墙）与 1,000 万 USD FDV 整数关口共振支撑区。
  - **风控接管声明**：严禁人工心算具体止盈止损价格点位或固定百分比；二级建仓后的动态止盈、回撤保护与斐波那契扩展位追踪，全权委托底部 `trailing-guard` 动力学哨兵按 `Wave A/B/C` 实时 K 线结构自动接管。
- **生态工具与一级衍生机会 SOP（针对 Robinhood Chain 发射台与节点租赁）**：
  1. 若无意直接承担 NFT 席位价格波动（0.65 ETH 至 1.99 ETH），可通过 `imdlend.com` 免押金或低成本租用他人闲置席位，在独立沙盒环境（Mac/Linux）挂载空闲 API 额度参与测试，实测单日奖励能否覆盖 API 成本；
  2. 重点监控 `imd.fun` Explorer 中基于 **Robinhood Chain** 新发布的合约/代币项目（Launches），利用其前端“仅显示 Hook 真实税率（shows only the tax its hook really takes）”的透明审计视图，筛选具备高销毁回馈的早期衍生标的。

### 🎯【RedKoi 实盘判定结论】
- 🔵 **[低投入 · 小资金试错(<=1%机动仓)/带退款保护打新]**
- **参与方式与撤退底线**：严禁在 FDV > 2,000 万 USD 或 NFT 席位溢价高点盲目追高重仓；建议采取“轻资产租席位实测 + 二级依托 POOL4 下方 ETH 买墙支撑区小仓位（<= 1% 机动仓）配置”的双轨策略，动态止损交由 `trailing-guard` 哨兵接管，一旦发现 `imdLend` 席位租赁活跃度连续两周萎缩、蜂群每日外部付费 Goal 订单枯竭或主网 `POOL4` 的 ETH 托底买墙被异常抽干，立即无条件清仓撤退。

---

## 📋 【任务交付成果 / 做了什么】
- **完成 `surfcoderepeat` (`imd.fun` / `IMD`) 全维度联网穿透取证**：通过多轮只读搜索核实了 `@surfcoderepeat`（Adam）系 Base 链知名应用 Fren Pet 联创的真实底细，查明该标的并非未发币空气项目，而是历经 `FP → VIBE → IMD` 演进、已部署以太坊主网合约（`0xd34a99bc0f67ae1bbd63c660e6d0b0dd03e263b7`）及 2,000 枚席位 NFT 的去中心化 AI Agent 蜂群协作网络。
- **穿透核心通缩机制与多链版图**：拆解了其基于 Uniswap v4 的 `POOL4`（`CappedBurnHook`）超额库存自动削减模型（85% 永久销毁 + 6% 算力补贴 + 4.5% sIMD 质押分红 + 4.5% NFT 节点奖励 + ETH 托底买墙），并核实其已原生打通 Ethereum、Base 与 Robinhood Chain 三链 RPC 与发射台回购销毁闭环。
- **严格执行 alpha-scout v2.1 规范交付完整研报**：完成动态 Loop 三步进阶审判、双脑会审红蓝交锋、大庄四维刑侦对账及 `Wave A/B/C` 波浪底座锚定，全文零违禁浮夸词、零裸美元与 LaTeX 符号。

## 💡 【决策动因 / 为什么这么做】
- **纠偏雷达 TRACK_B 分类错位，防范盲目当成零估值新盘打新**：雷达因抓取开发者月度功能总结推文将其归为 `TRACK_B_PRETOKEN`，若不深扒其 `FP → VIBE → IMD` 的前世今生，极易误判为尚未发币的处女盘而忽视其已达千万 USD 级 FDV 的历史筹码包袱。
- **落实第一性原理“主动自我设限”审查**：对比 Elysium 链寄生工具的短期提款跑路逻辑，Adam 团队通过 `CappedBurnHook` 将卖盘超额代币的 85% 硬编码销毁，且在过去 30 天高密度交付沙盒桌面端与跨链预言机，符合“克制短期快钱、做厚协议底座”的工程派特征，因此给予 `🔵 [低投入]` 的结构化参与评级而非一刀切否决。

## 👉 【后续行动 / 接下来需要 RedKoi 做什么】
- **无需手动介入，研报已全自动验证生效**：本工单系纯投研穿透任务，已在严格遵守只读安全红线的前提下完成闭环交付。
- **实盘观察建议（可选）**：若计划参与其生态，可先在测试机或闲置 Mac/Linux 沙盒环境中访问 `http://imd.fun/skill.md` 与 `imdlend.com`，核算租赁单个 Agent 席位的净收益比（奖励产出 vs Claude/Venice API 消耗成本）。

## 🎯 【参谋建议 / 小吴推荐与后续防线】
- **优先关注“铲子生态衍生机会”而非高价买断 NFT 席位**：当前 OpenSea 上 Identity.md 席位地板价处于 0.65 ETH 至 1.99 ETH 区间，回本周期受蜂群外部发单量制约；通过 `imdLend` 智能合约按需租用席位或关注其在 Robinhood Chain 上新开启的无代币合约/Launchpad 标的，赔率优于直接重仓买断高价 NFT。
- **严守证伪回滚底线**：将主网 `POOL4` 的 ETH 托底买墙储备量与每日活跃 Goal 数量作为核心生命线指标；若节点算力补贴无法覆盖外部 API 成本导致在线 Worker 节点数跌破活跃阈值，或二级价格跌破 `Wave C` 买墙支撑底座并触发 `trailing-guard` 止损信号，须坚决执行离场纪律。

---

#### 🛡️【移动风控全权委托契约 (Trailing-Guard Handover · 严禁研报心算点位)】
*【单职原则与系统解耦铁律 · 蓝图 134 v2.0 动力学定案】本技能核心职责是穿透大前提、基本盘、宏观资金与大庄博弈论，并输出波浪底座候选 (Wave A/B/C) 与做市池真实深度；研报内部严禁人工心算或硬编码任何固定百分比止盈止损点位！一旦用户在二级市场实际建仓成交，直接调用移动止盈止损技能 (`trailing-guard`)：*
```bash
python3 /root/pi-data/scripts/universal_trailing_sentinel.py add --key surfcoderepeat --ca surfcoderepeat --chain robinhood --symbol SURFCO --entry-mc <ENTRY_MC> --cost-usd <COST> --tokens <TOKENS> --wave-a <WAVE_A> --wave-b <WAVE_B> --wave-c <WAVE_C> --liquidity <LIQUIDITY_USD>
```
*由哨兵联动 `sr_analyzer.py` 根据真实成交均价、做市池真实深度与三点波浪结构自主求解动力学斐波那契点位（Wave A +1.5% 结构硬止损、1.272 斐波那契 TP1 卖出 40% 回笼 80% 本金、50% 动能衰竭中点锁利、35× 底池上限 R2 极端阻力墙、40% 纯利润仓单调递增 Trailing Stop 放飞）并纳管，杜绝机械固定百分比与纸上谈兵。*

