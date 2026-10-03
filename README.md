# Daily Routines 本地化文本存储仓库

**源语言文件**：`ChineseSimplified.json` 
**译文**：其他以 `.json` 结尾的语言文件

## 提交原文/译文

- 修改对应的 `.json` 文件，提交 **Pull Request**。合并后自动工作流会将原文与译文上传至 [Transifex](https://explore.transifex.com/dailyroutines/dailyroutines/)。
- 在 [Transifex](https://explore.transifex.com/dailyroutines/dailyroutines/) 上直接提交对应语言的译文。
- 提交新字符串时，请勿同时提交任何翻译文本，仅允许修改并提交**简体中文**字符串。

## 格式要求

- 所有非用于显示的英文名称（模块内部名称等）均遵循**大驼峰命名原则**，且不应该在内部包含任何标点符号（如下划线、连词符等）。
- 使用 **ICU Message Format** 标准进行格式化。
  ※ 部分资源仍在使用 `{0}`、`{2}` 此类的简单格式化，但仅出于兼容考虑而**暂时**保留，未来随时有可能将其改写为现行格式。
  ※ 简体中文原文一般因为**不需要**而无法见到各类 ICU Message Format 语法，但各语言译文可以根据需要编写复杂的表达式。
  ※ 一般类型传入全部**符合字面直觉**。即一个名为 `{level}` 的占位符其传入的就是数字，否则会将占位符命名为 `{levelText}`。当然也可以直接去查询使用该字符串的代码。

### 键

- 模块标题：`<模块内部名称>Title`（例：`FastObjectInteractTitle`）
- 模块描述：`<模块内部名称>Description`（例：`FastObjectInteractDescritpion`）
- 模块内部语言：`<模块内部名称>-<具体名称>`（例：`FastObjectInteract-AddToBlacklist`）
    - 注：可以使用形如 `Commands-CommandHelp-FavOn` 的格式来更加清晰地分类你的本地化键。

### 值

- 请勿让占位符实际传入各类查**游戏表**获得的值，会有较大的性能问题。
  ※ 部分资源仍有此类做法，但仅出于兼容考虑而**暂时**保留，未来随时有可能将其改写为现行格式。

**简体中文**

- 请根据现代汉语标准规范使用标点符号。
- 中英文混排需要以半角空格间隔。
- 中文数字混排依据实际用途决定：
    - 若用于游戏内聊天消息输出、原生界面文本等，中间不加任何半角空格。
    - 若用于 ImGui 绘制的界面（含 Dalamud 通知），推荐加入半角空格以提升清晰度。
- 若为完整句子，句末需要加句号。

**英文**

- 模块标题：所有单词的首字母均应大写 (例：`Fast Object Interaction`)