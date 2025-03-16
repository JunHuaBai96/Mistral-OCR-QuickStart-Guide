# Mistral OCR 初步使用指南

## 简介
本项目旨在提供Mistral OCR的初步使用指南，帮助用户快速上手并应用该OCR技术。

## 目录
1. 注册并获取 API-KEY
2. 安装
3. 使用
4. 参考来源
5. 许可证

## 注册并获取 API-KEY
1. 访问 [Mistral Console](https://console.mistral.ai/home) 并注册登录。
2. 点击"Set up my plan"，选择左边的体验免费计划。
3. 勾选相关选项，然后点击“Subscribe”。
4. 输入移动电话号码，点击“Send verification code via SMS”，等接收到短信验证码后输入验证码，检验通过。
5. 点击页面左侧导航栏的"API Keys"，然后点击右上角的“Create new key”，创建 api-key。

## 安装
安装好 Python 环境后，安装 mistralai 库：
```bash
pip install mistralai -i https://pypi.org/simple
```

## 使用
项目中已提供 `main.py` 文件，以下是使用说明：

1. 将 `main.py` 文件与待转换的 PDF 文件置于同一目录。
2. 修改 `main.py` 中的以下内容：
   - `"此处填写你的 api key"`：替换为你创建的 api key。
   - `"此处填写你要转换的 pdf 文件的文件名"`：替换为你的 PDF 文件名（如 `demo.pdf`）。
3. 运行以下命令：
   ```bash
   python main.py > demo.md
   ```
4. 程序运行完毕后，目录下会生成一个 `demo.md` 文件，即为转换后的 Markdown 文件。

## 参考来源
本文参考了知乎文章：[Mistral OCR 初步使用指南](https://zhuanlan.zhihu.com/p/28801320889)，感谢原作者的分享和贡献。

## 许可证
本项目采用 MIT 许可证，详情请见 [LICENSE](LICENSE) 文件。
