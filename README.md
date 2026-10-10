# SauceDemo 功能测试实战

## 📖 项目简介
基于 SauceDemo 电商网站进行功能测试实战，覆盖登录、商品列表、购物车、结算四大核心模块，共设计 33 条测试用例，发现 6 个缺陷。

## 🛠️ 技术栈
- 测试类型：功能测试、UI测试、性能测试
- 测试工具：浏览器 F12 开发者工具、Chrome Performance 面板
- 文档工具：Excel、Markdown

## 📂 项目结构
- `docs/`：测试计划、测试用例、测试报告
- `bugs/`：Bug列表（Excel + Markdown双版本，含截图）
- `screenshots/`：缺陷截图

## 🐛 发现的缺陷
| Bug编号 | 标题 | 严重程度 |
| :--- | :--- | :--- |
| BUG-001 | problem_user商品图片全部错乱 | 中 |
| BUG-002 | problem_user加购按钮功能异常 | 高 |
| BUG-003 | performance_glitch_user登录LCP达5.02秒 | 中 |
| BUG-004 | visual_user商品列表排版错位 | 低 |
| BUG-006 | problem_user排序功能失效 | 中 |
| BUG-008 | problem_user商品详情页加购按钮无响应 | 高 |

## 🔑 测试账号
| 用户名 | 密码 | 特点 |
| :--- | :--- | :--- |
| standard_user | secret_sauce | 正常用户 |
| locked_out_user | secret_sauce | 被锁定 |
| problem_user | secret_sauce | 含多个缺陷 |
| performance_glitch_user | secret_sauce | 加载缓慢 |
| visual_user | secret_sauce | UI错乱 |

## 💡 项目亮点
- 覆盖等价类、边界值、异常场景的完整用例设计
- 使用 Chrome Performance 面板量化性能问题（LCP 5.02s）
- 规范的缺陷管理流程，含复现步骤与截图证据
- 测试用例与Bug列表双向追溯