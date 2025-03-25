# Daily Routines 本地化文本存储仓库

**源语言文件**: `ChineseSimplified.json` 
**译文**: 其他以 `.json` 结尾的语言文件

## **提交原文/译文:**

- 修改对应的 `.json` 文件, 提交 **Pull Request**, 合并后自动工作流会将原文与译文上传至 [Transifex](https://explore.transifex.com/dailyroutines/dailyroutines/)
- 在 [Transifex](https://explore.transifex.com/dailyroutines/dailyroutines/) 上直接提交对应语言的译文

## 格式要求

所有非用于显示的英文名称 (如模块内部名称、具体名称等) 均遵循 **大驼峰命名原则**, 且不应该在内部包含任何标点符号 (如下划线、连词符等)

### 键

- 模块标题: `<模块内部名称>Title` (例: `FastObjectInteractTitle`)
- 模块描述: `<模块内部名称>Description` (例: `FastObjectInteractDescritpion`)
- 模块内部语言: `<模块内部名称>-<具体名称>` (例: `FastObjectInteract-AddToBlacklist`)
    - 注: 可以使用形如 `Commands-CommandHelp-FavOn` 的格式来更加清晰地分类你的本地化键

### 值

- 所有逗号 `，`, 冒号 `：`, 括号 `（）`, 方头括号 `【】` 均应使用它们各自的半角版本
- 中英文混排时, 应该使用一个半角空格分隔, 例: `你好 Test 你好` 或 `你好 Test, 你好`
- 使用逗号或冒号时, 仅后方紧跟一个半角空格, 例: `你好: Test`
- 使用其他标点符号时, 前后均应紧跟一个半角空格, 例: `你好 ———— 你好` 或 `你好 (表示问候)`
- 模块标题 (仅英文): 所有单词的首字母均应大写 (如: `Fast Object Interaction`)

## **翻译讨论:**

- 请直接新建一个 **Issue**, 以 `[对应语言] 主题` 的格式命名标题

## **注:**

- 若你为模块作者, 且正在提交一个新模块的本地化文本, 请勿提交除原文 (一般为简体中文) 外的任何翻译文本, 新模块的所有文本均需要进行质量检查以及改写与规范化, 提交翻译文本会带来额外的工作量