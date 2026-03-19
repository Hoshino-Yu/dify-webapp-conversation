# 对话式 Web 应用模板

这是一个基于 [Next.js](https://nextjs.org/) 开发的项目，使用 [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app) 初始化。

## 应用配置

在当前目录下创建一个名为 `.env.local` 的文件，并从 `.env.example` 复制内容。设置以下环境变量：

```env
# APP ID: 您的应用唯一标识符。
# 您可以在应用详情页面的 URL 中找到它。
# 例如：URL 为 `https://cloud.dify.ai/app/xxx/workflow`，则 `xxx` 就是您的 APP ID。
NEXT_PUBLIC_APP_ID=

# APP API Key: 用于验证应用 API 请求的密钥。
# 您可以在应用页面的“API 访问”栏目中，点击右上角的“API 密钥”按钮生成。
NEXT_PUBLIC_APP_KEY=

# APP URL: API 的基础地址。
# 如果您使用的是 Dify 云服务，请设置为：[https://api.dify.ai/v1](https://api.dify.ai/v1)
NEXT_PUBLIC_API_URL=