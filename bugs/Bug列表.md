# SauceDemo Bug 列表

> 测试平台：https://www.saucedemo.com/
> 测试时间：2026-10-10
> 测试环境：Windows 11 + Chrome 浏览器

---

## BUG-001：problem_user 商品图片全部错乱

| 字段 | 内容 |
| :--- | :--- |
| **模块** | 商品列表 |
| **严重程度** | 中 |
| **关联账号** | `problem_user` / `secret_sauce` |
| **复现步骤** | 1. 打开 saucedemo.com<br>2. 用 problem_user 登录<br>3. 查看商品列表页 |
| **预期结果** | 每个商品显示对应的图片 |
| **实际结果** | 所有商品显示同一张 404 占位图 |
| **状态** | 新建 |

**截图：**

![BUG-001](screenshots/BUG-001_problem_user_图片错乱.png)

---

## BUG-002：problem_user 加购按钮功能异常

| 字段 | 内容 |
| :--- | :--- |
| **模块** | 购物车 |
| **严重程度** | 高 |
| **关联账号** | `problem_user` / `secret_sauce` |
| **复现步骤** | 1. 用 problem_user 登录<br>2. 在商品列表点击 "Add to cart" |
| **预期结果** | 商品成功加入购物车，按钮变为 "Remove" |
| **实际结果** | 按钮无反应或商品未加入购物车 |
| **状态** | 新建 |

**截图：**

![BUG-002](screenshots/BUG-002_problem_user_加购失效.png)

---

## BUG-003：performance_glitch_user 登录加载超过10秒

| 字段 | 内容 |
| :--- | :--- |
| **模块** | 登录 |
| **严重程度** | 中 |
| **关联账号** | `performance_glitch_user` / `secret_sauce` |
| **复现步骤** | 1. 打开 saucedemo.com<br>2. 用 performance_glitch_user 登录 |
| **预期结果** | 3 秒内完成登录并跳转 |
| **实际结果** | 登录耗时超过 10 秒，页面明显卡顿 |
| **状态** | 新建 |

**截图：**

![BUG-003](screenshots/BUG-003_performance_glitch_登录慢.png)

---

## BUG-004：visual_user 商品列表排版错位

| 字段 | 内容 |
| :--- | :--- |
| **模块** | 商品列表 |
| **严重程度** | 低 |
| **关联账号** | `visual_user` / `secret_sauce` |
| **复现步骤** | 1. 用 visual_user 登录<br>2. 查看商品列表页 |
| **预期结果** | 图片和文字对齐整齐 |
| **实际结果** | 图片和文字错位、重叠 |
| **状态** | 新建 |

**截图：**

![BUG-004](screenshots/BUG-004_visual_user_排版错位.png)

---

## BUG-005：error_user 结算流程报错

| 字段 | 内容 |
| :--- | :--- |
| **模块** | 结算 |
| **严重程度** | 高 |
| **关联账号** | `error_user` / `secret_sauce` |
| **复现步骤** | 1. 用 error_user 登录<br>2. 添加商品到购物车<br>3. 进入结算流程 |
| **预期结果** | 正常完成下单，显示 "Thank you for your order!" |
| **实际结果** | 页面报错或流程卡住 |
| **状态** | 新建 |

**截图：**

![BUG-005](screenshots/BUG-005_error_user_结算报错.png)