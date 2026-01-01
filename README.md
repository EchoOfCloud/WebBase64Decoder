# Web Base64 Decoder

一个功能强大的基于Web的Base64解码器工具，可快速将Base64编码字符串转换为原始文本或二进制数据。

**本项目基于 MATE.tools 进行修改和扩展。**

## 功能特点

- **双模式解码**：支持单条模式和批量模式
- **智能数据检测**：自动识别解码结果是文本还是二进制数据
- **灵活批量处理**：支持自定义分隔符，默认使用换行符
- **多样化输出选项**：复制到剪贴板或下载为文件
- **响应式设计**：适配各种设备屏幕尺寸
- **纯前端实现**：数据处理安全可靠，无需服务器交互
- **友好的用户界面**：基于Bootstrap框架，简洁直观

## 技术栈

- **HTML5**：页面结构
- **CSS3**：样式设计
- **JavaScript**：核心功能实现
- **Bootstrap 5**：UI框架
- **jQuery 3.7.1**：DOM操作

## 目录结构

```
Base64解码器网页 可解码输出文件/
├── css/
│   ├── bootstrap-icons.min.css    # Bootstrap图标样式
│   ├── bootstrap.min.css          # Bootstrap核心样式
│   └── style.css                  # 自定义样式
├── images/
│   ├── mate.png                   # 图片资源
│   └── thumbs.db                  # 系统缩略图数据库
├── js/
│   ├── bootstrap.bundle.min.js    # Bootstrap JS捆绑包
│   └── jquery-3.7.1.min.js        # jQuery库
├── index.html                     # 主页面文件
├── README.md                      # 项目说明文档
├── 测试文件1：批量数据解密.csv     # 测试数据文件
└── 测试文件2：base64解密输出为压缩包文件.txt  # 测试数据文件
```

## 使用方法

### 单条模式

1. 在"Input Base64 String"文本框中粘贴Base64编码字符串
2. 点击"Decode Base64"按钮进行解码
3. 解码结果将显示在"Decode Result"区域
4. 可选择"Copy to Clipboard"复制结果，或"Download as File"下载文件

### 批量模式

1. 选择"Batch Mode"选项
2. 在"Delimiter"输入框中设置分隔符（可选，默认为换行符）
3. 在"Input Base64 String"文本框中输入多条Base64编码字符串，每条占一行或用指定分隔符分隔
4. 点击"Decode Base64"按钮进行批量解码
5. 解码结果将合并显示在"Decode Result"区域

### 下载文件

1. 在解码前或解码后，在"Filename"输入框中输入自定义文件名（可选）
2. 点击"Download as File"按钮将解码结果保存为文件

## 使用示例

### 示例1：解码文本

输入：
```
SGVsbG8gV29ybGQh
```

输出：
```
Hello World!
```

### 示例2：批量解码

输入：
```
SGVsbG8gV29ybGQh
SGVsbG8gQmFzZTY0IQ==
```

输出：
```
Hello World!
Hello Base64!
```

## 注意事项

1. 确保输入的Base64字符串完整且有效
2. 对于二进制数据，解码后将显示"Binary content detected. Use download button to save file."
3. 批量模式下，空行将被自动忽略
4. 自定义分隔符支持转义序列，如`\n`（换行）、`\t`（制表符）、`\r`（回车）
5. 建议使用现代浏览器（Chrome、Firefox、Safari、Edge）以获得最佳体验

## 浏览器兼容性

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## 本地部署

1. 克隆或下载项目文件到本地
2. 直接在浏览器中打开`index.html`文件即可使用
3. 也可以通过本地Web服务器（如Apache、Nginx）部署

## 测试数据

项目包含两个测试文件，可用于验证工具功能：

- `测试文件1：批量数据解密.csv`：包含批量Base64编码数据
- `测试文件2：base64解密输出为压缩包文件.txt`：包含二进制文件的Base64编码

## 许可证

本项目采用MIT许可证，详见LICENSE文件。

## 贡献

欢迎提交Issue和Pull Request来改进项目。

## 联系方式

如有问题或建议，欢迎通过以下方式联系：

- 项目地址：[GitHub Repository]
- 电子邮件：[your-email@example.com]

---

**Web Base64 Decoder** - 简单、高效、安全的Base64解码工具