# SDKURL 加速服务

> 通过反向代理官方SDK，让中国大陆用户免加速器登录。

---

## 加速地址

| 原始地址 | 加速地址 |
|---------|---------|
| `https://jp-sdk-api.yostarplat.com`| `https://jp-sdk-api.bluearchive.help` |

---

## 使用方法

替换`src/index.js`里的请求地址即可：

```diff
- https://jp-sdk-api.yostarplat.com
+ https://jp-sdk-api.bluearchive.help
```

请注意，您需要自行配置`wrangler.jsonc`，以适配您的CF服务。

---

## 已知问题

游戏API地址：

```
https://prod-game.bluearchiveyostar.com:5000/api/
```

该接口不在加速范围内。

部分地区访问此API会因网络问题失败（包括非客户端请求），如出现网络不稳定则需使用VPN或加速器或等待一段时间即可。
