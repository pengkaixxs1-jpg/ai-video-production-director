# AI Video Production Director

一个面向 AI 视频制作的 Codex skill，用于把创意、剧情、分镜、首帧/关键帧、生图提示词、视频提示词或失败结果，整理成可生成、可继承、可审查的专业视听生产方案。

它不是简单的提示词润色器，而是一套从镜头功能、物理因果、角色表演、切镜逻辑、连续性管理和失败诊断出发的 AI 视频生产方法。

## What It Helps With

- 将一句创意扩展为完整 AI 视频方案
- 拆解首帧、生图提示词、视频提示词和镜头尾状态
- 设计动作、打戏、逃跑、摔倒、接触、支点和反应链
- 管理多镜头之间的人物、道具、伤势、光源和环境痕迹连续性
- 修复“电影感不足”“动作漂浮”“角色漂移”“道具突然出现”“切镜随机”等常见问题
- 把失败结果沉淀成可复用的项目规则和负面约束

## Core Ideas

1. 功能先于漂亮：每个镜头必须知道自己承担什么叙事、动作、信息或情绪功能。
2. 结构先于审美：空间、支点、接触点、首尾状态不成立时，不靠风格词补救。
3. 证据先于解释：真实、压迫、危险、神圣、疲惫、电影感，都要落到可见、可听、可继承的参数。
4. 继承先于爽点：上一镜的姿态、伤势、道具、环境痕迹、声音尾巴和焦点债务，需要在下一镜被处理。
5. 参数选择先于堆叠：每次只选择三到五个主模块，其余保持底线约束。

## Install From GitHub

This repository stores the skill at the repository root. Use `--path .` and explicitly set the skill name.

### Windows PowerShell

```powershell
python "$env:USERPROFILE\.codex\skills\.system\skill-installer\scripts\install-skill-from-github.py" --repo pengkaixxs1-jpg/ai-video-production-director --path . --name ai-video-production-director
```

### macOS / Linux

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py --repo pengkaixxs1-jpg/ai-video-production-director --path . --name ai-video-production-director
```

After installation, restart Codex to pick up the new skill.

If the repository is private, the installer needs GitHub access through existing git credentials or a `GITHUB_TOKEN` / `GH_TOKEN`. For public use, make the repository public first.

## How To Use

In Codex, ask for the skill by name:

```text
使用 ai-video-production-director，把下面这个短片想法拆成首帧、生图提示词、视频提示词、切镜逻辑和质检清单：
一个受伤的机械臂少女在暴雨废墟中逃离追捕。
```

Or in English:

```text
Use $ai-video-production-director to turn this AI video idea into a grounded shot plan, image prompt, video prompt, continuity plan, and QA checklist:
A wounded courier crosses a flooded industrial tunnel while drones search overhead.
```

## Example Output Shape

The skill usually returns:

- task function diagnosis
- visual evidence package
- image prompt / first-frame prompt
- video prompt
- shot or panel breakdown
- continuity locks
- sound and dialogue anchors
- negative constraints
- QA score and failure patches

## Repository Structure

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── action-chain.md
    ├── continuity-patches.md
    ├── cutting-logic.md
    ├── image-prompt-framework.md
    ├── production-framework.md
    └── qa-and-diagnosis.md
```

## Reference Modules

- `production-framework.md`: general AI video production logic and parameter systems
- `image-prompt-framework.md`: still image, first frame, character sheet and storyboard prompt logic
- `action-chain.md`: body action, support, contact, reaction and physical constraints
- `cutting-logic.md`: edit points, attention debt, axis, omission and montage
- `continuity-patches.md`: object pre-existence, character anti-drift and mechanical structure conservation
- `qa-and-diagnosis.md`: scoring, red lines, failure diagnosis and reusable patch deposition

## Good Use Cases

- AI video prompt engineering
- image-to-video planning
- multi-shot continuity design
- character trailer planning
- anime or cinematic storyboard development
- generated video failure review
- project-level prompt methodology building

## Design Principle

The skill treats AI video as a controllable audiovisual production process:

```text
idea -> function -> evidence -> frame -> action -> continuity -> generation prompt -> QA -> reusable patch
```

The goal is not to make prompts longer. The goal is to make every word carry production responsibility.
