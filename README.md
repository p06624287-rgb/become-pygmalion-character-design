# 成为皮格马利翁—角色设计

**Become Pygmalion — Character Design · by AIR · v1.0.0**

一套由 AI 直接承担图像制作的角色设计 Skill。从一句角色想法、故事或参考图出发，逐步完成画风、头脸、身体比例、服装、道具与最终设定；既可以专注产出，也可以在制作中学习设计判断。

> Ciallo～(∠・ω< )⌒★，这里是AIR的角色设计，接下来我们将进行角色设计的全流程，赋予ta真正的生命，准备好了吗？

每个新角色项目首次启动时展示这句开场词，同一项目的续作和修改不重复。

## 两种模式

| 模式 | 适合谁 | 工作方式 |
| --- | --- | --- |
| 生产模式 | 希望直接获得角色成果 | AI制作图像，简述判断，重点确认关键方向与最终结果 |
| 产学模式 | 希望边做边学习角色设计 | AI同样负责出图，通过可比较方案讲解观察方法、选择依据和修改效果 |

两种模式共用质量标准，都执行“生成 → 看图评审 → 修订或确认 → 推进”，不把大量细节或高分辨率当成设计进步。用户可以随时切换模式，已有确认成果不会被重置。

## 设计流程

1. 选择模式，再询问是否需要3D模型。
2. 盘点故事、人设、已有角色图或喜欢的参考；没有完整故事也可以开始。
3. 建立简洁角色任务书，区分身份参考、设计灵感、画风与结构依据。
4. 缺参考时按人设在Pinterest检索，实际看图后提供来源与选择理由。
5. **先确定主画风，再进入大量角色设计和精修。**
6. 整体方向 → 头脸与身体基准 → 服装及核心道具 → 全身整合与配色。
7. 按用途制作表情、动作、服装差分和连续性测试，不强制每个项目做全套。
8. 交付最终立绘、所需设定图及轻量记录；需要作品集时整理真实关键过程。

已有合格设计从缺口继续，不要求重画。重要参考记录“借什么、为什么适合角色、如何转译”，不把外部角色整套复制当作原创设计。

## 安装与调用

这是Codex Skill指令包，不是独立绘图软件。

下载仓库后，将包含`SKILL.md`的目录命名为`become-pygmalion-character-design`，放到你的Codex用户skills目录，保持`agents/`与`references/`的相对位置。如果已有同名版本，先备份并检查差异，不盲目覆盖。

也可以将本仓库链接交给具备skill安装能力的助手，明确请求安装。工具安装依照使用者环境和权限执行。

调用示例：

```text
使用 $become-pygmalion-character-design，帮我开始角色设计。
```

也可以提供已有条件：

```text
使用 $become-pygmalion-character-design。我选择产学模式，不需要3D。
我只有一个角色想法，希望先找参考、确定画风，再开始设计。
```

## 工具需求与三维边界

- 图像生成与编辑能力：AI需要实际出图，不只交提示词。
- 浏览或图像搜索能力：用于缺失参考与必要的文化、材料研究；无法访问时会明确说明。
- 本地文件能力：用于保留图像、版本和轻量记录。
- 3D为可选：未选择就不安装、不启动、不上传任何三维任务。

选择3D后，全部三维环节交接 **[Charakuru官方Skill](https://github.com/nanocle/Charakuru)**，从[官方发布页](https://github.com/nanocle/Charakuru/releases)下载安装，并按实际安装版本的官方规则使用。

本仓库不包含Charakuru源代码、原Skill、安装包、素体或三维操作脚本，不复制其技术流程，也不以自建Tripo/Blender路线替代。Charakuru自身的人工审核、许可、环境要求与外部服务费用独立适用。本项目与Charakuru并无官方隶属或背书关系。

## 文件结构

```text
become-pygmalion-character-design/
├── SKILL.md
├── agents/openai.yaml
├── references/design-workflow.md
├── references/project-record.md
├── README.md
├── LICENSE
└── .gitignore
```

主规则负责开场、模式、约束和路由；工作流说明阶段图像与评审；记录模板只在用户项目中按需使用。不要把项目图片、个人聊天、凭据和本地工作记录提交回本仓库。

## 当前验证状态

v1.0.0的核心4个技能文件已完成官方格式校验、UTF-8及中文名称检查、开场词精确核对、资源引用检查和安装副本一致性检查；另外完成了静态场景走查。

**尚未完成使用本Skill制作新角色的端到端实测。** 格式正确不保证生成图质量；静态设定不等于可用动画，安装Charakuru也不等于完成3D模型。不同宿主的工具、费用与网络条件会影响执行。

欢迎通过Issue反馈可复现的问题，或提交针对性的改进。反馈请说明模式、阶段、预期与实际结果；不要上传密码、令牌、私人聊天或无权分享的角色素材。

## 许可证

本仓库原创指令与文档采用[MIT License](LICENSE)，版权署名为 **AIR**。

此许可不扩展至Charakuru、其他第三方工具、用户输入素材或生成结果中的第三方权利。相关素材与服务仍须遵守各自许可及条款。

---

An AI-assisted character-design Skill by AIR, with production and learning modes. It prioritizes early style selection, reference transformation, direct image generation, staged visual review, and reusable character assets. Optional 3D work is delegated exclusively to the separately installed official Charakuru workflow. No third-party code or private character assets are bundled.
