# TradeCilent - Minecraft 商城与交易插件<Badge type="tip" text="Latest: 3.7.4" />



## 简介

TradeCilent 是一个为Minecraft服务器设计的交易插件，支持玩家开设个人商店，进行商品买卖，并提供了一系列管理功能。此外，还包含了资金组系统以及贷款机制，为服务器增添了更多经济互动元素。

## 特性

- 开设个人商城GUI，展示并管理上架物品。
- 支持多种交易操作：上架、下架、购买商品。
- 提供详细的资金统计和个人资产查看。
- 强大的管理员工具：商品管理和用户权限控制。
- 资金组系统允许玩家组成团队共同管理资金。
- 玩家可以向服务器申请贷款，体验真实的经济体系。

## 安装指南

### 服务器端安装

1. 下载 `TradeCilent.jar` 文件并放置于服务器的 `plugins` 文件夹内。
2. 启动或重启服务器以加载插件。
3. 配置 `config.yml` 文件（位于 `plugins/TradeCilent/`）来调整插件行为。

### 客户端无需安装任何内容，直接在服务器中使用即可。

## 使用方法

### 基本指令

- `/shopgui`: 打开商城界面。
- `/Tradecilent onsell <itemname> <amount> <price>`: 上架商品。
- `/Tradecilent downsell <itemname> <amount>`: 下架商品。
- `/Tradecilent buy <itemname> <playername>`: 购买指定玩家的商品。
- `/Tradecilent info profit`: 查看今日盈利。
- `/Tradecilent info expenses`: 查看今日开销。
- `/Tradecilent info ranking`: 查看排行榜。
- `/Tradecilent info <@s/playername> money`: 查看个人总资金信息。

### 管理员指令

- `/Tradeop banitem <playername> <playeritem>`: 强制下架商品。
- `/Tradeop priceitem <playername> <playeritem>`: 修改商品价格。
- `/Tradeop bantrade <playername>`: 禁止玩家使用插件指令。
- `/Tradeop unbantrade <playername>`: 恢复被禁止玩家的权限。
- `/Tradeop delatemoney <playername> <amount>`: 扣除玩家资金。
- `/Tradeop givemoney <playername> <amount>`: 给予玩家资金。
- `/Tradeop setmoney <playername> <amount>`: 设置玩家资金。

### 服务器经济指令

- `/servereconomic`: 查看服务器总资产及黑名单人数等信息。

### 资金组和交易指令

- `/transaction give <playername> <amount>`: 给予某人资金。
- `/transaction auto accept/refuse`: 自动接受或拒绝资金。
- `/transaction group [<player1> <player2> ...]`: 创建资金组。
- `/transaction groupsave <amount>`: 向资金组存钱。
- `/transaction kickgroup <playername>`: 踢出资金组成员。
- `/transaction disband`: 解散资金组。
- `/transaction out <amount>`: 成员从资金组取款。
- `/transaction joinaccept`: 同意新玩家加入资金组。
- `/transaction outaccept`: 同意成员取出资金。
- `/transaction br <amount> <time>`: 申请贷款。
- `/transaction back`: 还款。
- `/transaction brinfo`: 查看贷款信息。

**注意**: 

`<itemname>` 可以为物品名称或 ID, `<playername>` 可以为在线玩家标识符如 `@s`, `@a`, `@r`, `@e`；`<amount>` 为低精度浮点数；`<time>` 为整数天数。

## 配置

编辑 `plugins/TradeCilent/config.yml` 文件来自定义插件行为，包括但不限于商城GUI布局、资金组规则等。

## 常见问题解答

- 将问题发送至邮箱: <2105165021@qq.com>
- 在社区解答: 进入qq群 952518546

## 贡献

欢迎任何形式的贡献！前往网站 [https://docs.amethyst.icu](https://docs.amethyst.icu) 或是进入qq群 952518546 参与讨论。

## 致谢
感谢以下人员对本项目的支持：
 - silence_cm_39 : 插件制作者本尊
 - StarrySkyWorld : 服务器项目的总指挥，首领，是@silence_cm_39的导师，对该项目提供了大量支持。
 - color : 就是个打杂的，为什么把他写到md里面呢，为了凑字数。

## 关于本项目的一些信息

- 本项目不开源，属于闭源插件
- 您只有使用权，禁止通过`任何手段`获取本项目的源代码/Jar 包。
- 如有任何疑问，请联系作者：<2105165021@qq.com>