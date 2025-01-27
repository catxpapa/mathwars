# 视觉界面
我希望UI布局在大多数情况下总是分为两个主要部分，一个部分是情景和氛围的表现，主要是可变化的层叠图像或视频，另一部分是操作或说明区，用来与用户进行主要交互。这样这两个区在竖屏可以上下排布，横屏可以左右排布，不会因画面比例变化太大而难以呈现。另外的元素如背景、操作区、技能栏、状态栏等，都以不同的层次浮动并自适应画面，必要时收缩一些内容，比如把按钮汇集成菜单。

图片素材将尽可能用AI生成，也就是说主要为静态的位图，但是可能用工具处理成背景透明或矢量化。以便多层叠加起来给画面增加可变因素或基于CSS特效的简单动画，也可能会包含一些同样用AI生成的视频动画或特效素材等。
# 用户体验
面向的主要用户是5-12岁的学龄儿童，更大的年轻人和成年人也可以参与，但是在成绩排行和成就设计时要考虑到划分不同的年龄段区域，以免更高年龄的玩家碾压低年龄玩家的成绩。

游戏主线应该是可持续及可扩展的，文字不适宜太长，可以用地图、场景画面或动画表达情节。

具体每个挑战应该是较快节奏，比如在5-10分钟可以完成一局。除了答题区的呈现之外，还需要有类似游戏的动效、氛围、音乐音效、激励动画等元素的考虑。根据不同的呈现特点，可以有主线任务、支线任务、日常任务等类别。

界面应该与传统游戏不同，而是更像用游戏元素美化过的传统应用，可以自适应不同设备，也可以适应横屏或竖屏、桌面键鼠及触控设备等。

界面的皮肤应该易于更换，以便衍生出更多的知识领域（世界）及更利于本地化（比如图片元素的多语言版本）

# 设计说明
主界面模块
1. 情景和氛围表现区

素材规格：动态背景图像或视频，建议使用高分辨率（至少1920x1080）以确保在不同设备上清晰呈现。
种类：AI生成的静态位图、透明背景图、矢量图形，可能包含简单的CSS特效动画。
操作或说明区

素材规格：应包含按钮、文本框和说明文字，按钮尺寸建议为宽度150px，高度50px，文本框应适应内容长度。
种类：可交互的UI组件，如按钮、下拉菜单、文本输入框，使用SVG或PNG格式的图标。

2. 用户交互模块
答题区

素材规格：题目展示区域应支持多行文本，建议使用可变字体大小以适应不同屏幕。
种类：题目文本、选项按钮（可选择的答案），可使用AI生成的图标或图像作为选项的视觉辅助。
反馈和评分区

素材规格：动态评分显示，建议使用动画效果来增强用户体验。
种类：分数显示文本、奖励动画（如星星、勋章等），可以使用GIF或SVG格式。

3. 任务和成就模块
任务列表

素材规格：每个任务的展示框应支持图标和文本，建议宽度300px，高度100px。
种类：任务图标、任务描述文本，使用PNG或SVG格式的图标。
成就展示

素材规格：成就展示区域应支持多个成就的并排显示，建议每个成就框宽度150px，高度150px。
种类：成就图标、描述文本，使用AI生成的图标或图像。

4. 其他辅助模块
背景和音效

素材规格：背景音乐和音效文件应为高质量音频，建议使用MP3或WAV格式。
种类：游戏背景音乐、按钮点击音效、任务完成音效。
多语言支持

素材规格：文本内容应支持多语言版本，建议使用JSON格式存储不同语言的文本。
种类：各语言的文本资源文件。

5. 适应性设计
响应式布局
素材规格：所有模块应支持自适应设计，确保在横屏和竖屏模式下均能良好展示。
种类：使用CSS媒体查询和灵活的布局设计，确保不同设备上的用户体验一致。

# 素材规格
| 用图类型       | 图片说明                         | 接受格式       | 尺寸建议                |
| -------------- | -------------------------------- | -------------- | ----------------------- |
| 背景图         | 用于主界面或情景展示的背景图像   | JPG, PNG, GIF  | 至少1920x1080像素       |
| 按钮图标       | 用于操作按钮的图标               | SVG, PNG       | 150x50像素              |
| 任务图标       | 每个任务的视觉辅助图标           | PNG, SVG       | 100x100像素             |
| 成就图标       | 展示成就的图标                   | PNG, SVG       | 150x150像素             |
| 选项图标       | 答题区选项的视觉辅助图标         | PNG, SVG       | 50x50像素               |
| 动态效果图     | 用于反馈和评分的动态效果图       | GIF, APNG      | 适应内容，建议不超过300x300像素 |
| 音效图标       | 用于音效按钮的图标               | PNG, SVG       | 50x50像素               |
| 多语言文本图   | 显示不同语言的文本图             | PNG            | 根据文本长度调整        |
