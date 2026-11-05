# 生态呼吁：为什么币安 Web3 钱包与 BAW 应当尽快接入 HyperEVM (Chain ID 999)？
> **作者**: RedKoi Research (@redkoi_eth) | **发布日期**: 2026-11-05
> **GitHub Issue 提案**: https://github.com/binance/binance-skills-hub/issues/407

---

### 一、引言：Web3 钱包的生态版图与缺失的拼图

币安 Web3 钱包（Binance Web3 Wallet）凭借其极致的安全风控、便捷的 MPC 门限签名与庞大的用户体量，已经成为全球数千万用户探索链上 DeFi、铭文、Meme 与 AI 智能体的核心入口。尤其近期推出的 Binance Agentic Wallet (`baw`) CLI 工具，更是将 AI 智能体自主调用链上钱包的能力推向了工业级前沿。

然而，在当前的链上多链实战中，一个日益严峻的痛点正在困扰着广大用户与 AI 开发者：**币安 Web3 钱包及 BAW 目前尚未支持 HyperEVM（Chain ID 999，Hyperliquid 官方 EVM 链）**。

今天，我们正式在币安官方开源社区提交了 Feature Request 提案（Issue #407），并在此从生态、技术与用户体验三重视角，深度剖析为何币安应当尽快官方接入 HyperEVM。

---

### 二、现实痛点：MPC 门限白名单下的“资产显示与转出困局”

随着 Hyperliquid 生态的爆发，大量用户通过第三方跨链桥（如 Relay）将 Base、Arbitrum 上的 ETH/USDT 跨入 HyperEVM 网络。

#### 1. 链上成功到账，但钱包 UI 形成“视觉盲区”
当用户将跨链目标地址填写为其币安 Web3 钱包的 EVM 地址时，链上底层交易已通过 Secp256k1 椭圆曲线完美确权，资金毫秒级安全进入该地址。但在手机端币安 App 的 Web3 钱包中，由于网络列表中没有 HyperEVM，用户完全无法看到自己的 HYPE 资产与链上余额，引发了大量的恐慌与客服咨询成本。

#### 2. MPC 签名白名单硬拦截，导致“只进不出”
币安 Web3 钱包为了极致的安全合规，采用了服务端参与的 MPC 门限签名机制。目前币安签名服务端对公链 Chain ID 施加了严格的白名单管控（仅放行以太坊、BSC、Base、Polygon、Arbitrum、Optimism、Avalanche 等 7 条 EVM 链）。
当用户或 AI 智能体尝试在 HyperEVM (Chain ID 999) 上发起转账或调用智能合约时：
```bash
baw wallet balance --binanceChainId 999
# 触发报错: Unsupported chain or chain not recognized
```
由于 Chain ID 999 被拦截在签名网关之外，用户无法在不导出原生私钥的情况下直接转出或调度该资产，严重影响了资金的流动性与用户体验。

---

### 三、战略价值：HyperEVM 为什么是币安不可忽视的必争之地？

#### 1. 庞大的生态沉淀与真实交易量
Hyperliquid 是当前 Web3 链上衍生品与自主 L1 赛道无可争议的领军者：
- **TVL 规模**：全网沉淀资金超过 3 亿美元；
- **日交易体量**：永续合约与现货日交易额屡破 10 亿美元；
- **HyperEVM 上线**：为这个原本就具备微秒级撮合能力的高性能 L1 赋予了原生的 EVM 组合性，使得海量 DeFi、借贷、去中心化稳定币与原生 Meme 爆发式涌现。

#### 2. AI Agent（智能体经济）的最佳土壤
币安通过 BAW 率先布局 AI Agent 链上钱包，而 HyperEVM 凭借其极低的 Gas 费、确定性的高速出块与深厚的订单簿流动性，正是 AI 算法进行自动化高频对冲、套利与资产托管的天然温床。如果 BAW 能够官方原生支持 HyperEVM，将直接赋能全球 AI 开发者在这一顶级流动性网络中跑通智能体闭环。

---

### 四、技术可行性：极度标准化，改造成本趋近于零

HyperEVM 完全遵循以太坊官方标准规范，没有任何非标准魔改：
* **Chain ID**：`999`
* **原生代币**：`HYPE`（18 位精度）
* **RPC 接口**：`https://rpc.hyperliquid.xyz/evm`
* **协议标准**：完全兼容 EIP-155、EIP-1559、JSON-RPC 2.0 与标准 ERC-20 / ERC-721
* **区块浏览器**：Hypurrscan (`https://hypurrscan.io`)

对于币安工程团队而言，在 MPC 服务端签名校验逻辑中新增 `999` 白名单放行，并在 App 前端与 BAW 配置文件中补充 RPC 节点映射，所需的工作量极小，但带来的生态口碑与用户留存价值不可估量。

---

### 五、给币安 Web3 团队的明确建议

1. **App 端接入**：在币安 Web3 钱包的“添加自定义网络”或官方默认支持网络中，将 HyperEVM (Chain ID 999) 纳管，支持资产可视化；
2. **MPC 签名放行**：在 MPC 签名网关中放行 Chain ID 999 的交易签名请求；
3. **BAW CLI 升级**：在 npm `@binance/agentic-wallet` 中原生集成 `--binanceChainId 999`，为全球 Web3 AI 开发者铺平道路。

**我们呼吁币安官方团队倾听社区与开发者的真实呼声，早日上线对 HyperEVM 的全面支持！**

---
*声明：本文由 RedKoi Research 独立撰写，旨在推动 Web3 多链互通与开发者生态建设，不构成任何投资建议。*
