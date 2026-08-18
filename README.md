# 车易付充电运营平台 - 对账管理（本地副本）

## 来源
- 原始地址：https://cheyifu-reconciliation.surge.sh/
- 复制日期：2026-08-18

## 文件结构

### platform_copy/ — 平台对账页面
- `platform.html` — 对应 https://cheyifu-reconciliation.surge.sh/platform.html#/list
  - 标题：车易付充电运营平台 - 对账管理（微信即充即退版）
- `sdk-seed.js` — Kimi 脚本（原 https://www.kimi.com/sdk-seed.js，已本地化）

### merchant_copy/ — 商户对账页面
- `merchant.html` — 对应 https://cheyifu-reconciliation.surge.sh/merchant.html
  - 标题：车易付充电运营平台 - 商户与平台业务订单对账

## 说明
- 两个页面均为自包含单页应用（内联 CSS + JS），无需额外依赖即可在本地打开运行
- platform.html 原引用的外部脚本 sdk-seed.js 已下载到本地并更新引用路径
- 原始源地址未做任何修改，这是独立的本地副本

## 本地预览
用浏览器直接打开 HTML 文件即可：
- 平台对账：platform_copy/platform.html
- 商户对账：merchant_copy/merchant.html

或用本地服务器：
```bash
cd outputs
python3 -m http.server 8080
# 访问 http://localhost:8080/platform_copy/platform.html#/list
# 访问 http://localhost:8080/merchant_copy/merchant.html
```
