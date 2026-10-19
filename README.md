# Love From Dog

MIMOMO & JIGOGO 的聊天空间。默认与“汤”的 AI 分身聊天，“牛顿的火焰激光剑”的 AI 分身暂未开放。头像来自本人指定的两张图片，聊天右侧的用户头像使用小鸟。

这里仅包含静态网页。模型权重、LoRA、训练数据、微信聊天、访问密钥和聊天数据库都保存在本地电脑。

## GitHub Pages

将本目录中的文件上传到 `Lucky-pig-cedar/Love_From_Dog` 的 `main` 分支根目录。
打开仓库 **Settings → Pages**，选择 **Deploy from a branch → main → /(root) → Save**。
部署地址为 `https://lucky-pig-cedar.github.io/Love_From_Dog/`。

实际聊天请使用电脑上网站服务生成的完整分享链接，其中包含进入权限。页面从 endpoint.json 读取当前 HTTPS 模型接口，不把权限密钥放入这个公开文件。不要把完整邀请链接或密钥提交到公开仓库。

GitHub Pages 不运行模型。电脑端须保持网站后端和原 GGUF 模型连接运行；当前使用人格 skill 与 RAG，LoRA 暂停使用，女朋友模型等待后续明确同意。
当前模型接口使用临时 Cloudflare Tunnel。已配置的本机同步脚本在网站启动、通道地址变化后更新 endpoint.json；GitHub 入口及其带 key 的邀请链接可以保持相同。同步依赖本机 GitHub 登录仍有效，发布有延迟。固定后端域名尚未配置；模型及本机服务仍须在线。

聊天记录按浏览器设备分别保存到本地数据库。清理浏览器存储或换设备后不会自动恢复原设备的历史。
