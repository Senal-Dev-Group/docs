# Senal 做市商 API 文档

Senal 做市商 API 的技术文档，基于 [Mintlify](https://mintlify.com) 构建。

## 文档结构

```text
├── index.mdx                    # 简介
├── quickstart.mdx               # 快速上手
├── authentication.mdx           # 认证（L1 EIP-712 + L2 HMAC-SHA256）
├── concepts/                    # 核心概念
│   ├── order-types.mdx          # 订单类型（GTC/GTD/FOK/FAK）
│   ├── heartbeat.mdx            # 心跳机制
│   └── websocket.mdx            # WebSocket 概述
├── api-reference/               # API 参考
│   ├── overview.mdx             # API 概览
│   ├── auth/                    # 认证接口
│   ├── orders/                  # 订单接口
│   ├── trades/                  # 成交接口
│   ├── markets/                 # 市场接口
│   ├── account/                 # 账户接口
│   ├── heartbeat/               # 心跳接口
│   └── websocket/               # WebSocket 频道
│       ├── overview.mdx         # 连接、认证、订阅
│       ├── orderbook.mdx        # 订单簿频道
│       ├── trade.mdx            # 成交频道
│       ├── orders.mdx           # 订单频道（私有）
│       └── positions.mdx        # 持仓频道（私有）
└── docs.json                    # Mintlify 配置
```

## 本地开发

```bash
# 安装 Mintlify CLI
npm i -g mintlify

# 启动开发服务器
mintlify dev
```

访问 `http://localhost:3000` 预览。

## 部署

推送到 `main` 分支后自动部署到 Mintlify。
