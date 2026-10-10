# SauceDemo Bug 列表

> 测试平台：https://www.saucedemo.com/
> 测试时间：2026-10-10
> 测试环境：Windows 11 + Chrome 浏览器
> 共发现缺陷：6 个

---

## BUG-001：problem_user 商品图片全部错乱

| 字段 | 内容 |
| :--- | :--- |
| **模块** | 商品列表 |
| **严重程度** | 中 |
| **关联用例** | TC-014 |
| **关联账号** | `problem_user` / `secret_sauce` |
| **复现步骤** | 1. 打开 saucedemo.com<br>2. 用 problem_user 登录<br>3. 查看商品列表页 |
| **预期结果** | 每个商品显示对应的图片 |
| **实际结果** | 所有商品显示同一张 404 占位图 |
| **状态** | 新建 |

**截图：**
![BUG-001](../screenshots/BUG-001_image_broken.png)

---

## BUG-002：problem_user 加购按钮功能异常

| 字段 | 内容 |
| :--- | :--- |
| **模块** | 购物车 |
| **严重程度** | 高 |
| **关联用例** | TC-022 |
| **关联账号** | `problem_user` / `secret_sauce` |
| **复现步骤** | 1. 用 problem_user 登录<br>2. 在商品列表点击 "Add to cart" |
| **预期结果** | 商品成功加入购物车，按钮变为 "Remove" |
| **实际结果** | 按钮无反应或商品未加入购物车 |
| **状态** | 新建 |

**截图：**
![BUG-002](../screenshots/BUG-002_add_cart_fail.png)

---

## BUG-003：performance_glitch_user 登录 LCP 达 5.02 秒

| 字段 | 内容 |
| :--- | :--- |
| **模块** | 登录 |
| **严重程度** | 中 |
| **关联用例** | TC-031 |
| **关联账号** | `performance_glitch_user` / `secret_sauce` |
| **复现步骤** | 1. 用 performance_glitch_user 登录<br>2. 打开 Chrome F12 Performance 面板记录加载过程 |
| **预期结果** | 页面 LCP 应在 2.5 秒以内 |
| **实际结果** | 页面 LCP 达到 5.02 秒（红色 Poor 级别），加载明显卡顿 |
| **状态** | 新建 |

**截图：**
![BUG-003](../screenshots/BUG-003_login_slow.png)

---

## BUG-004：visual_user 商品列表排版错位

| 字段 | 内容 |
| :--- | :--- |
| **模块** | 商品列表 |
| **严重程度** | 低 |
| **关联用例** | TC-032 |
| **关联账号** | `visual_user` / `secret_sauce` |
| **复现步骤** | 1. 用 visual_user 登录<br>2. 查看商品列表页 |
| **预期结果** | 图片和文字对齐整齐 |
| **实际结果** | 图片和文字错位、重叠 |
| **状态** | 新建 |

**截图：**
![BUG-004](../screenshots/BUG-004_layout_broken.png)

---

## BUG-006：problem_user 排序功能失效

| 字段 | 内容 |
| :--- | :--- |
| **模块** | 商品列表 |
| **严重程度** | 中 |
| **关联用例** | TC-034 |
| **关联账号** | `problem_user` / `secret_sauce` |
| **复现步骤** | 1. 用 problem_user 登录<br>2. 下拉选择 "Price (low to high)" |
| **预期结果** | 商品按价格升序排列 |
| **实际结果** | 排序无任何变化 |
| **状态** | 新建 |

**截图：**
![BUG-006](../screenshots/BUG-006_sort_fail.png)

---

## BUG-008：problem_user 商品详情页加购按钮无响应

| 字段 | 内容 |
| :--- | :--- |
| **模块** | 商品详情 |
| **严重程度** | 高 |
| **关联用例** | TC-035 |
| **关联账号** | `problem_user` / `secret_sauce` |
| **复现步骤** | 1. 用 problem_user 登录<br>2. 进入任意商品详情页<br>3. 点击 "Add to cart" |
| **预期结果** | 商品加入购物车，按钮变为 "Remove" |
| **实际结果** | 按钮无反应，购物车角标不更新 |
| **状态** | 新建 |

**截图：**
![BUG-008](../screenshots/BUG-008_detail_add_fail.png)