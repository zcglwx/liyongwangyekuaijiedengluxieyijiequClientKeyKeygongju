# 利用网页快捷登录协议截取ClientKey、Key工具

## 工具简介

本工具是针对最新的腾讯QQ客户端版本(9.7.20)设计的，实现了利用网页快捷登录协议来捕获和分析用户电脑上已登录QQ的相关安全密钥信息，如ClientKey、Skey、P_skey等。这一过程通过一系列精心设计的步骤完成，旨在教育和研究目的，了解此协议的工作原理。

### 实践学习资源
详细的实战教程可在[CSDN博客](https://blog.csdn.net/qq_39190622/article/details/129489268?spm=1001.2014.3001.5501)找到，教程以中文进行，包含完整的教学内容与源代码分享，适合对网络协议、网络安全及QQ快捷登录机制感兴趣的开发者学习。

### 工具功能分解

1. **初始化与会话建立**：工具首先配置初始访问地址，发送请求，并从中解析出`pt_local_token`。
   
2. **QQ UIN获取**：利用第一步得到的`pt_local_token`，构建新URL请求，进而获取当前已登录QQ的uin号码。

3. **ClientKey截取**：结合`pt_local_token`和已知的uin，发起特定请求，实现ClientKey的获取。

4. **Skey与ptsigx提取**：在成功获得ClientKey之后，进一步操作以获得Skey，并从中提取必要的ptsigx值。

5. **最终获取P_skey**：最后，工具通过之前步骤收集的信息构造请求，最终完成P_skey的获取。

## 注意事项

- **仅供学习与研究**：请确保您合法合规地使用此工具，不得用于侵犯他人隐私或非法活动。
- **软件兼容性**：本工具专门适配于QQ版本9.7.20，对于其他版本可能不完全适用。
- **技术教育目的**：强烈建议在理解相关网络协议和安全原则的基础上使用，促进技术知识的学习与交流。

---

本README.md提供了关于“利用网页快捷登录协议截取ClientKey、Key工具”的简要指南，旨在帮助用户理解其用途与操作流程，务必在合法范围内应用技术成果。

## 下载链接
[利用网页快捷登录协议截取ClientKeyKey工具](https://pan.quark.cn/s/75f8a28153df) 

(备用: [备用下载](https://pan.baidu.com/s/19b1ejGWneT9buF9Iwrf06g?pwd=1234))

## 说明

该仓库仅用于学习交流，请勿用于商业用途。
