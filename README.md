# AINiangAssets

AI 角色 2D 形象与视频素材库。本仓库为**素材存档**，非"已完成/可发布"验收；成片、动作与抠图质量需另行人工审阅。

## 目录结构

```
2d/
  portraits/          21 位角色双形态立绘（<id>-dual.png）
  action-atlas/       84 张动作图（<id>-{chibi|anime}-{walk|scenes}.png）
  fullbody/           deepseek + claude 全身立绘与骨骼绑定源图（anime/chibi，含 zip）
  cutouts/            Feiyu 桌宠/互动站抠图与 Chibi（deepseek/claude/gemini/gpt/grok）
  chibi-references/   Qwen/GLM/Kimi/MiniMax 的 Chibi 参考图
videos/<id>/          每位角色 20 个透明 WebM 动作（首批，字母序前 20）
```

## 角色 ID ↔ 角色名（权威源 `ainiang/output/characters.json`）

| ID | 角色名 | | ID | 角色名 | | ID | 角色名 |
|---|---|---|---|---|---|---|---|
| deepseek | 大肥鱼 | | qwen | 千金金 | | mistral | 风芒 |
| gpt | 小龙女 | | kimi | 小狐狸 | | hunyuan | 元汐 |
| claude | 圣女果 | | glm | 嘎拉吗 | | llama | 绒原 |
| gemini | 哈基米 | | minimax | 小田螺 | | step | 阶音 |
| grok | 大小姐 | | doubao | 豆暖 | | muse | 缪光 |
| | | | mimo | 米澄 | | novelai | 绘咏 |
| | | | cohere | 珂据 | | seedance | 镜禾 |
| | | | zcode | 霜栈 | | opencode | 墨端 |

## 素材来源（provenance）

| 仓库路径 | 来源（Feiyu 工作区） |
|---|---|
| `2d/portraits/` | `ainiang/output/images/<id>-dual.png` |
| `2d/action-atlas/` | `ainiang/output/action-atlas-v1/sheets/*.png` |
| `2d/fullbody/` | `ainiang/output/2d-fullbody-v2/`（source + zip + manifest） |
| `2d/cutouts/` | `assets/characters/**` |
| `2d/chibi-references/` | `productions/ai-pets-200/references/<Id>-Chibi.png` |
| `videos/<id>/` | `productions/ai-pets-200/runs/<id>/webm/`（DeepSeek 源目录为 `runs/feiyu/`） |

## 说明

- **视频为首批**：每位角色 20 个透明 WebM（按文件名字母序取前 20）。完整动作集（`productions/ai-pets-200/runs/`，9 位各约 141–200 条）因总量约 7.5GB 未整体入库，后续按需分批补充。
- **DeepSeek 资产 ID**：素材源用 `feiyu`，本仓库统一为权威 ID `deepseek`。
- **视频覆盖 9 位**：deepseek / claude / gemini / gpt / grok / qwen / glm / kimi / minimax；其余 12 位（doubao / mimo / cohere / mistral / hunyuan / llama / step / muse / novelai / seedance / zcode / opencode）暂无视频。
