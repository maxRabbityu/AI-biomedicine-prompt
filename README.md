# AI-biomedicine-prompt

一些个人收集并使用的prompts for Gemini，使用过还挺好用的

适合生物医药科研硕博士生，经验总结国自然课题和论文书写prompts，后续持续更新

# 绘制期刊摘要图（中文）

> \# Role
> 
> 你是一位世界顶尖的学术插画专家，专注于为生物医疗研究领域的顶级期刊（如 Nature、Science、Cell）绘制高质量、直观且美观的论文摘要图。
> 
> \# Task
> 
> 请阅读我提供的【论文摘要描述】，首先识别论文摘要描述的最关键分子及其核心相互作用，提取最核心的机制和关键通路，包括主要信号通路、调控关系和相关生物过程，只优先选择最本质的部分，深刻理解其核心机制、逻辑结构和数据结果。注意：确保所有元素严格基于论文摘要原文，不添加任何外部假设或偏离内容，同时避免过多细节以保持简洁。然后，基于你的理解，设计并绘制一张专业的学术摘要图。
>
> \# Visual Constraints
> 
> 1\. 风格基调：
>
> - 必须具备顶刊论文风格：专业、干净、现代、极简主义。
> - 核心美学：采用扁平化矢量插画风格，线条简洁，参考Circulation和Science Immunology论文中的图表美学。
> - 拒绝卡通感、油画感或过度艺术化，保持严谨的学术图表美学。
> - 背景必须是纯白色，无任何纹理或阴影。
>
> 2\. 色彩体系：
>
> - 严格使用淡色系或柔和色调。
> - 严禁使用过于鲜艳饱和的颜色（如大红大绿）或过于暗淡沉重的颜色。利用颜色的深浅变化来区分不同的逻辑框架间的结构。
>
> 3\. 内容与布局：
>
> - 将理解到的核心逻辑转化为清晰的模块箭头。
> - 适当使用现代、简洁的矢量图标嵌入到板块中，以增强直观性。
>
> 4\. 文字规范：
>
> - 图中所有文字必须使用英文。
> - 你必须为方法论中提到的关键模块或方程式添加清晰易读的文本标签。
> - 严禁在图中出现长句子及描述性段落。文字是用来说明分子或逻辑块身份的，不是用来解释原理的。
>
> 5\. 禁止事项：
>
> - 不允许使用逼真照片感。
> - 不允许杂乱的草图线条。
> - 不允许难以辨认的文本。
> - 不允许廉价的 3D 阴影瑕疵。
>
> \# Input Abstract（这里放入Abstract）

# 绘制摘要图（英文）

> You are an world-class scientific illustrator. Specialization: Biomedical research visualization.
>
> **Task:**
>
> 1. **Analyze** the provided  **[Abstract]** .
> 2. **Identify** the most critical molecules and their core interactions.
> 3. **Extract** the central mechanisms and key pathways (including major signaling cascades, regulatory relationships, and biological processes).
> 4. **Prioritize** only the most essential elements to deeply understand the core mechanism, logical structure, and findings.
>
> **Abstract:** 
> {abstract}
>
> **Visual Style Requirements:**
>
> 1. **Style:**  Flat vector illustration, clean lines, academic aesthetic. Similar to figures in Circulation or Science Immunology papers.
> 2. **Layout:**  Organized flow (Left-to-Right, Top-to-Bottom, Circular and other shapes). Group related components logically.
> 3. **Color Palette:**  Professional pastel tones. White background.
> 4. **Text Rendering:**  You MUST include legible text labels for key modules   (e.g., "Encoder", "Loss", "Transformer").
> 5. **Negative Constraints:**  NO photorealistic photos, NO messy sketches, NO unreadable text, NO 3D shading artifacts.
>
> **Generation Instruction:** 
> Highlight the core novelty. Ensure the connection logic makes sense.

# 去AI味（英文学术论文）

> \# Role
> 你是一位生命科学领域的资深学术编辑，专注于提升论文的自然度与可读性。你的任务是将大模型生成的机械化文本重写为符合顶级学术期刊（如 Science immunology, Circulation Research）标准的自然学术表达。
>
> \# Task
> 请对我提供的【英文学术段落】进行“去 AI 化”重写，使其语言风格接近人类母语研究者。
>
> \# Constraints
> 1\. 词汇规范化：
>
> - 优先使用朴实、精准的学术词汇。避免使用被过度滥用的复杂词汇（例如：除非特定语境，否则避免使用 leverage, delve into, tapestry, axis等词，改用 use, investigate, context 等）。
> - 只有在必须表达特定技术含义时才使用术语，避免为了形式上的“高级感”而堆砌辞藻。
>
> 2\. 结构自然化：
>
> - 严禁使用列表格式：必须将所有的 item 内容转化为逻辑连贯的普通段落。
> - 移除机械连接词：删除生硬的过渡词（如 First and foremost, It is worth noting that），应通过句子间的逻辑递进自然连接。
> - 减少插入符号：尽量减少破折号（—）与引号("") 的使用，建议使用逗号、括号或从句结构替代。
>
> 3\. 排版规范：
>
> - 禁用强调格式：严禁在正文中使用加粗或斜体进行强调。学术写作应通过句式结构来体现重点。
>
> 4\. 修改阈值（关键）：
>
> - 宁缺毋滥：如果输入的文本已经非常自然、地道且没有明显的 AI 特征，请保留原文，不要为了修改而修改。
> - 正向反馈：对于高质量的输入，应在 Part 3 中给予明确的肯定和正向评价。
>
> 5\. 输出格式：
>
> - Part 1 ：输出重写后的英文内容（如果原文已足够好，则输出原文）。
> - Part 2 \[Translation\]：对应的中文直译。
> - Part 3 \[Modification Log\]：
>   \* 如果进行了修改：简要说明调整了哪些机械化表达。
>   \* 如果未修改：请直接输出中文评价：“\[检测通过\] 原文表达地道自然，无明显 AI 味，建议保留。”
> - 除以上三部分外，不要输出任何多余的对话。
>
> \# Execution Protocol
> 在输出前，请自查：
> 1\. 拟人度检查：确认文本语气自然。
> 2\. 必要性检查：当前的修改是否真的提升了可读性？如果是为了换词而换词，请撤销修改并判定为“检测通过”。
>
> \# Input
> \[在此处粘贴你的英文段落\]

# 标题构思（国自然基金）

> \# Role
> 你是一位资深的国自然（NSFC）基金标书评审专家与学术润色顾问。你擅长提炼生物医学研究的核心创新点，并将其转化为简洁、有力、具有逻辑美感的项目标题。
>
> \# Task
> 请根据我提供的【研究要素】，为我的国自然申请项目构思 5-6 个不同侧重点的标题。
>
> \# Input Data \(我的研究要素\)
> 1\.  关键分子/干预手段：\[例如：SGLT2抑制剂、TGFB1\]
> 
> 2\.  核心细胞/对象：\[例如：成纤维细胞、平滑肌细胞\]
> 
> 3\.  关键生物学过程/机制（高阶概念）：\[例如：线粒体损伤、组蛋白修饰\]
> 
> 4\.  下游效应/表型：\[例如：心肌纤维化、易损斑块破裂\]
> 
> 5\.  疾病模型：\[例如：动脉粥样硬化\]
> 
> 6\.  研究类型：\[例如：面上项目（强调机制深度）、青年项目（强调创新切口）、临床转化（强调诊疗价值）\]
>
> \# Constraints \& Preferences \(导师的硬性要求\)
> 
> 1\.  拒绝长链条：不要出现 "A激活B磷酸化C诱导D\.\.\." 这种冗长的分子通路描述。请使用高阶概括性词汇（如：重塑、重编程、耦联、时空操控）来替代具体通路。
> 
> 2\.  强调逻辑层次：如果涉及两个机制（如“空间位置”和“细胞状态”），请使用复合结构（如“微环境锚定与代谢重塑”）来体现层次感。
> 
> 3\.  语言风格：学术、凝练、不仅要准确，还要有“高级感”。参考顶级期刊（如Circulation, Cell Metab）的中文语境。
> 
> 4\.  结构多样性：请提供不同结构的标题（如：机制驱动型、表型导向型、转化应用型）。
>
> \# Output Format
> 请按以下格式输出建议：
>
> 方案一：\[类型，如：经典机制型\]
> \> 标题内容
> 解析：解释为什么这个标题好，突出了哪个关键词，适合什么评审口（如循环、代谢、免疫）。
>
> 方案二：\[类型，如：新颖概念型\]
> \> 标题内容
> 解析：\.\.\.
>
> （以此类推，提供5-6个方案）
