# English:

# CDN-Origin-Pull-IP-Extractor

CDN-Origin-Pull-IP-Extractor is a tool for extracting origin-pull IP addresses from CDN access logs. Since obtaining origin-pull IPs from most major CDN providers requires payment and some smaller CDN providers do not offer this feature, this tool aims to help users conveniently extract CDN origin-pull IPs (CDN node ≠ CDN return to source node) by analyzing log content.


## Online Demo

[🔗 View Demo](https://www.rockaz.top/CDN-Origin-Pull-IP-Extractor)  
Note: The website server is located in China. For security defense purposes, all traffic outside China has been blocked.


## Function Description

- Supports analysis and origin-pull IP extraction for two common log formats
- Displays extracted IP addresses grouped by network segments, facilitating the identification of IP segment patterns
- Provides two input methods: direct log content entry or file upload
- Supports one-click copying of analysis results for subsequent use


## Supported Log Formats

1. **Leichi WAF Access Logs**  
   The log path is usually: Protected Applications > Application Details > Application Logs.  
   The tool will extract the first IP address in each log line as the origin-pull IP.

2. **NCSA Standard Format Logs**  
   Applicable to logs following the NCSA standard, such as Alibaba Cloud ESA.  
   The tool will analyze and extract all IP segments with similar prefixes to identify potential origin-pull IP segments.


## Usage Method

1. Download the `CDN-Origin-Pull-IP-Extractor.html` file from the repository to your local device.
2. Open the HTML file with any modern browser (e.g., Chrome, Firefox, Edge, etc.).
3. Select the corresponding tab ("Leichi WAF Logs" or "NCSA Standard Logs") according to your log type.
4. Enter log content or upload a log file:
   - Direct input: Paste log content into the text box.
   - File upload: Click "Select File" to upload a log file with the extension `.log` or `.txt`.
5. Click the "Analyze" button under the corresponding tab ("Analyze Leichi Logs" or "Analyze NCSA Logs").
6. View the analysis results: Results will be displayed grouped by IP segments, including the number of IPs in each segment and specific IP addresses.
7. To save the results, click the "Copy Results" button, and the results will be copied to the clipboard.


## Notes

- Log content must be complete and conform to the corresponding format; otherwise, extraction results may be inaccurate.
- The tool runs only in the local browser and does not upload log content to servers, ensuring data privacy.
- Extraction results are for reference only; actual origin-pull IPs may change due to CDN provider configuration adjustments.


## License

This project is open-sourced under the Apache-2.0 license. For details, please refer to the LICENSE file. When using it, please comply with the open-source agreement; unauthorized tampering with copyright information is prohibited.


## Source

This tool's code is based on the original page code from [Rockaz.top](https://www.rockaz.top/CDN-Origin-Pull-IP-Extractor), with streamlining and optimizations (external JS references removed and styles replaced for better user experience).


# 中文：

# CDN-Origin-Pull-IP-Extractor

CDN-Origin-Pull-IP-Extractor 是一个用于从CDN访问日志中提取回源IP地址的工具。由于多数大厂CDN的回源IP获取需要付费，而部分小厂CDN未提供该功能，本工具旨在通过分析日志内容，帮助用户便捷地提取CDN回源IP（CDN节点≠CDN回源节点）


## 在线演示

[🔗 查看演示](https://www.rockaz.top/CDN-Origin-Pull-IP-Extractor)  
注：网站服务器位于中国境内，出于安全防御目的，已屏蔽中国境外所有流量


## 功能说明

- 支持两种常见日志格式的分析与回源IP提取
- 对提取的IP地址按网段分组展示，便于识别IP段规律
- 提供日志内容直接输入或文件上传两种方式
- 支持分析结果一键复制，方便后续使用


## 支持的日志格式

1. **雷池WAF访问日志**  
   日志路径通常为：防护应用 > 应用详情 > 应用日志。 
   工具会提取每行日志中第一个IP地址作为回源IP

2. **NCSA标准格式日志**  
   适用于阿里云ESA等遵循NCSA标准的日志。 
   工具会分析并提取所有具有相似前缀的IP段，识别可能的回源IP段。


## 使用方法

1. 下载仓库内的 `CDN-Origin-Pull-IP-Extractor.html` 文件到本地
2. 用任意现代浏览器（如Chrome、Firefox、Edge等）打开该HTML文件
3. 根据你的日志类型，选择对应的标签页（"雷池WAF日志"或"NCSA标准日志"）
4. 输入日志内容或上传日志文件：
   - 直接输入：在文本框中粘贴日志内容
   - 文件上传：点击"选择文件"，上传扩展名为 `.log` 或 `.txt` 的日志文件
5. 点击对应标签页下的"分析"按钮（"分析雷池日志"或"分析NCSA日志"）
6. 查看分析结果：结果会按IP段分组展示，包含每个网段的IP数量及具体IP地址
7. 如需保存结果，点击"复制结果"按钮，结果将被复制到剪贴板


## 注意事项

- 日志内容需完整且符合对应格式，否则可能导致提取结果不准确
- 工具仅在本地浏览器中运行，不会上传日志内容至服务器，保障数据隐私
- 提取结果仅供参考，实际回源IP可能因CDN厂商配置变更而变化


## 许可证

本项目基于 Apache-2.0 许可证开源，详情请参阅 LICENSE 文件；使用时请遵守开源协议，未经允许不得擅自篡改版权信息


## 来源

本工具代码基于 [Rockaz.top](https://www.rockaz.top/CDN-Origin-Pull-IP-Extractor) 的原页面代码精简优化（删除外部引入JS且更换样式，以便更好的让大家使用）而来
