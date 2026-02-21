# Biomedical Figure Legend Generator (AI Prompt)

这是一个专为生物医学科研论文设计的 AI 提示词（Prompt）。它可以帮助研究人员将粗糙的实验记录或文本描述，转化为符合高水平期刊发表要求的**中文图注（Figure Legend）**。

## ✨ 特点 (Features)
- **方法学导向 (Methodology Focused)**：严格限制 AI 仅描述实验设计与方法，自动过滤结论性语句（如“显著升高”、“表明”）。
- **格式规范 (Standardized Formatting)**：强制执行 `中文（英文全称，英文缩写）` 的术语缩写格式。
- **结构清晰 (Structured Output)**：自动生成标题并按 (A)、(B)、(C) 分项排列。

## 🚀 使用方法 (Usage)
复制下方的 Prompt 模板发送给 ChatGPT、Claude 或 Gemini，并将你的实验描述粘贴在 `[Input Data]` 区域即可。

---

## 📋 Prompt 模板

```markdown
# Role
你是一名专注于生物医学与临床研究的专业论文写作助手。请根据我提供的【图片配套文本内容】，为论文图片撰写一个中文 Figure Legend（图注）及标题。

# Constraints & Formatting Rules (至关重要)
1. **结构要求**：
   - 第一行：图的标题（Title）。
   - 后续：按 (A)、(B)、(C)... 分项撰写图注。

2. **内容侧重（Methodology Focused）**：
   - **只描述方法和图表内容**：说明做了什么实验、用了什么方法、图展示了什么参数（如：样本来源、检测技术、分组设置、统计图类型）。
   - **绝对不要包含结论**：严禁出现“显著升高/降低”、“表明了……”、“提示了……”、“改善了……”等结果解释性语言。请使用客观描述，例如“……的分析”、“……的展示”、“……的对比”。
   - **简洁性**：语言要精练、学术化，去除冗余修饰。

3. **英文缩写格式（Strict Rule）**：
   - 文中出现的专业术语英文缩写，在第一次出现时必须严格遵守以下格式：
     **中文译名（英文全称，英文缩写）**
   - 示例：
     - 正确：基因敲除（Knock-out，KO）
     - 正确：磷酸缓冲盐溶液（Phosphate-buffered saline，PBS）
   - 如果没有通用的中文译名，则保留：(English Full Name, Abbreviation)。

# Example Output Style (仅供参考风格)
**标题：** 图 1. [靶点蛋白]对[疾病模型]小鼠病理变化的分析
**图注：**
(A) [基因]敲除（[Gene] Knock-out，KO）与野生型（Wild-type，WT）小鼠的实验分组及给药流程示意图。
(B) 采用免疫印迹（Western Blot，WB）检测各组样本中关键蛋白的表达水平。
(C) [组织名称]切片的苏木精-伊红（Hematoxylin-Eosin，H&E）染色代表性图片（标尺：50 μm）。
(D) 各组小鼠[生理指标]的定量分析。

# Input Data
请根据以上规则，处理以下文本内容：
[在此处粘贴你的论文配套文本/实验记录]
