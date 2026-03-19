# 会话 Web 应用模板

这是一个基于 [Next.js](https://nextjs.org/) 的项目，使用 [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app) 初始化创建。

---

## 配置应用

在当前目录下创建一个名为 `.env.local` 的文件，并复制 `.env.example` 的内容。然后填写以下配置：

- **APP ID**：应用的唯一标识符。可以在应用详情页的 URL 中找到。  
  例如，在 URL  
  `https://cloud.dify.ai/app/xxx/workflow`  
  中，`xxx` 就是你的 APP ID。  
  ```env
  NEXT_PUBLIC_APP_ID=
APP API Key：用于认证应用 API 请求的密钥。
可以在应用的 “API Access” 页面右上角点击 “API Key” 按钮生成。
Env
复制代码
NEXT_PUBLIC_APP_KEY=
APP URL：API 的基础地址。
如果使用 Dify 云服务，设置为：
复制代码

https://api.dify.ai/v1
Env
复制代码
NEXT_PUBLIC_API_URL=
更多配置
在 config/index.ts 文件中进行配置：
Ts
复制代码
export const APP_INFO: AppInfo = {
  title: 'Chat APP',
  description: '',
  copyright: '',
  privacy_policy: '',
  default_language: 'zh-Hans'
}

export const isShowPrompt = true
export const promptTemplate = ''
快速开始
安装依赖
Bash
复制代码
npm install
# 或
yarn
# 或
pnpm install
启动开发服务器
Bash
复制代码
npm run dev
# 或
yarn dev
# 或
pnpm dev
打开浏览器访问：
复制代码

http://localhost:3000
使用 Docker
构建镜像
Bash
复制代码
docker build . -t <DOCKER_HUB_REPO>/webapp-conversation:latest
运行容器
Bash
复制代码
docker run -p 3000:3000 <DOCKER_HUB_REPO>/webapp-conversation:latest
打开浏览器访问：
复制代码

http://localhost:3000