# NGCC 新一代商用密码算法 · 公钥类第一轮候选速览

一个**单页静态站点**，把新一代商用密码算法（NGCC）全球征集**公钥类第一轮 84 个候选**整理成可检索、可筛选的清单，并附上**家族分类**与**规范要点摘要**。

- 数字签名 34 · 密钥封装（KEM）41 · 密钥交换（KEX）9
- 家族分布：格密码 43 · 编码类 22 · 哈希类 4 · MPC-in-the-Head 5 · 多变量 5 · 同源类 4 · 其他 1

## 内容

| 文件 | 说明 |
|---|---|
| `index.html` | 页面本体（原生 JS，无外部依赖，读取 `data.json` 渲染） |
| `data.json` | 结构化数据：名称、类别、家族、安全假设、规范要点、部分参数尺寸 |
| `standalone.html` | **自包含单文件版**（数据内嵌，双击即可离线查看，方便转发） |
| `preview.png` | 页面预览图 |

## 数据来源

- **候选名单**：官方公告的公开候选列表（公开信息）。
- **技术内容**：各提交方**公开发布**的算法规范文本；本仓库对其做了结构化摘录与归纳。
- 本仓库**不含任何个人信息**（无姓名、单位、邮箱、联系方式）。

## 免责声明

- 本仓库为**公开信息的整理与速览**，与征集组织方及任何提交方**无隶属或背书关系**。
- 摘录与分类由自动抽取加人工/模型校对完成，**可能存在遗漏、过时或不准确之处**；一切以官方公告与提交方原始规范为准。
- 本仓库**不构成**对任何算法的安全性评价、推荐或结论；涉及安全性的判断请参阅原始规范与独立分析。

## 本地使用

```bash
git clone <this-repo>
cd <this-repo>
python3 -m http.server 8000   # 然后浏览器打开 http://127.0.0.1:8000/
```

也可以直接双击打开 `index.html`（部分浏览器对本地 `fetch` 有限制时请用上面的本地服务器）。

## GitHub Pages

仓库根目录已包含 `.nojekyll`。在 **Settings → Pages** 中选择 `main` 分支、`/ (root)` 目录即可发布。

## 许可

见 [`LICENSE.md`](LICENSE.md)：数据与整理文本采用 CC BY 4.0，页面代码采用 MIT。

---

## English

A single-page static site listing the **84 first-round public-key candidates** of the NGCC
post-quantum standardization call, with family classification and structured summaries of the
publicly available specifications and submission material.

- No personal information is included (no names, affiliations, e-mail addresses or phone numbers).
- The content is a compilation of **publicly available** material; it may contain omissions or
  inaccuracies, and the official announcements / original specifications prevail.
- This repository is **not affiliated with** the organizing body or any submitter, and does **not**
  constitute a security evaluation or recommendation.

License: data and compiled text under CC BY 4.0; page code under MIT (see [`LICENSE.md`](LICENSE.md)).
