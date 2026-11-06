<!-- CURRICULUM-BUILDER-NOTES:START -->
<!-- 此段由 curriculum-builder 自动维护，请勿手动编辑分隔线之间的内容 -->

## 笔记写作规范

### Section 结构

每篇学习笔记必须包含以下 5 个 Section：

1. **一句话** — 核心思想的单句概括
2. **核心公式/原理** — 数学推导或关键图表
3. **与其他概念的关系**
   - 前置依赖（本课需要的前置知识）
   - 对比区别（与相似概念的区别）
   - 后续延伸（后续课程会用到本课的哪些点）
4. **关键来源** — 每个重要论断必须标注原始出处，禁止"无来源断言"
   - 论文: `[Author (Year), "Title"](URL), Venue`
   - 书籍: `《书名》第 X 章 — 作者, 出版社 (Year)`
   - 网页: `[文章标题](URL) — 网站名, YYYY-MM-DD`
   - 视频/课程: `[视频标题](URL) — 作者, 平台, YYYY-MM-DD`
   - AI 对话: `[话题] — Claude/GPT, YYYY-MM-DD ⚠️ 需人工验证`
5. **我的实验** — 动手验证记录（代码输出、实验结果等）

### 语法规则 (Obsidian)

| 元素 | 语法 |
|------|------|
| 内部链接 | `[[note-name]]` 或 `[[note-name\|显示文本]]` |
| Callout | `> [!note]` / `[!warning]` / `[!important]` / `[!success]` / `[!tip]` / `[!abstract]` / `[!question]` / `[!danger]` |
| Frontmatter | `---` 块: `tags`, `created`, `updated`, `status` |
| 外部链接 | `[Author (Year), "Title"](URL), Venue` |

### 状态流转

```
draft → reviewed → polished
```
- 写完初稿标记 `draft`
- 复习后更新 `updated` 日期，升为 `reviewed`
- 反复打磨后升为 `polished`

### 防偏规则

- **课前:** 确认前置依赖已满足，运行 `driver.py checklist --lesson X.Y`
- **课后:** 运行 `driver.py advance --lesson X.Y` 原子更新课程表
- **离题拦截:** 与当前 Lesson 无关的深度问题 → 简要回答(1-2句) + 标记延后评估，不立即展开教学
- **来源追溯:** AI 生成的内容必须标注为 AI 来源并建议人工验证，不可将 AI 输出伪装为确定事实
- **准入标准:** 新增课程需满足 ≥2/4 准入条件，不可因用户提问即时添加

<!-- CURRICULUM-BUILDER-NOTES:END -->
