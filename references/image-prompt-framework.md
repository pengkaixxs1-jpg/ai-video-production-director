# Image Prompt Framework

Use this reference for static image generation, first frames, keyframes, storyboard panels, multi-panel reference images, and any task where the output is a still visual prompt.

## Main Rule

Do not start by writing a beautiful prompt. Start by deciding what the image must prove.

Order of thinking:

1. Demand breakdown: subject, action, environment, image purpose.
2. Narrative function: what must this image establish?
3. Normal action system: support, grip, center of gravity, contact, motion stage.
4. Unit relation lock: independent, connected, nested, composite, causal, obstructed.
5. Frame position: left/right/up/down and foreground/midground/background.
6. Camera direction relative to subject.
7. Depth layers and spatial anchors.
8. Action and physical feedback.
9. Style anchor: extract visual temperament, not imitation.
10. Final prompt, targeted negative constraints, frozen moment.

Final prompt order:

`前置气质锚点 -> 画面总述 -> 剧情功能锁定 -> 正常动作系统 -> 单位关系锁定 -> 主体方位 -> 机位方位 -> 景深层级 -> 动作与物理反馈 -> 角色/道具/环境细节 -> 画面质感 -> 负面约束 -> 核心冻结状态`

## Narrative Function

Ask: why does this image exist in the story?

Common functions:

- Action threshold: about to release, draw, fire, pull, strike, or break.
- Pressure establishment: giant, monster, authority, god, or environment suppresses a weaker subject.
- Evidence close-up: prove one physical fact such as hand contact, blade scrape, wall mark, or wound.
- Spectacle generation: deity forming, time stop, mass weapons, abnormal weather.
- Character identity: first reveal of profession, status, temperament, or ability.
- Space establishment: prove field structure, scale, paths, and material reality.

The image is not merely a good-looking image; it is an image that carries a job.

## Normal Action System

When the user gives an action label, complete the physical action.

Fill:

- action purpose
- action stage: start, in progress, limit, after release
- center of gravity and support point
- limb division: which hand, foot, shoulder, waist does what
- contact point: hand-wall, foot-ground, knife-wall, arrow-string
- grip mode: forward grip, reverse grip, half grip, knuckle hook, palm heel support
- force direction: pull, push, press, twist, brace, diagonal impact, recoil
- feedback: dent, crack, tension, powder, spark, sleeve fold, skin pressure

Reject impossible limb tasks. One hand cannot fully palm a wall and fully grip a dagger at the same time. Rewrite as partial palm heel, tiger-mouth edge, finger back, or knuckle contact.

## Unit Relations

Complex images fail when the model fuses units. Lock unit relationships before composition.

Six relations:

1. **Independent units**: not the same object; should not merge. Example: blade and blade aura, person and shadow.
2. **Connected units**: different parts have connection points. Example: handle to blade, mechanical arm to shoulder socket.
3. **Nested/wrapped units**: one unit partly inside or around another. Example: blade inside sheath, body inside coat.
4. **Composite whole**: multiple parts form one system. Example: mechanical arm, firearm, armor, platform.
5. **Causal but not physical connection**: one unit triggers another result. Example: blade causes mountain crack light, but is not a long light sword.
6. **Obstruction relation**: overlap without fusion. Example: smoke half-obscures arm, barrel blocks fist.

Red line: if a relation would create a bizarre unestablished material form or break action, structure, or feedback, rewrite it.

## Frame-First Composition

Use frame coordinates before abstract meaning.

Required order:

1. Subject position: left/right/center, upper/middle/lower, foreground/midground/background, facing, key limbs and props.
2. Camera position: relative to subject, height, shot size, lens feel, purpose.
3. Depth layers: foreground obstruction, midground subject/prop, background light/exit/wall/mountain/anchor.
4. Action and state: path, support, center of gravity, contact, reaction, gaze, injury, physiology.
5. Visible details: appearance, clothing, weapon, material, blood, rain, dust, steam, electric arc.
6. Sound/tail state when the image is a keyframe for video.

Mantra: locate the subject in the frame, then locate the camera relative to the subject, then locate everything else.

## Realism and Texture System

Realism is not dirt, grayness, damage, or ugliness. Realism means light, color, material, space, force, motion feedback, and detail distribution follow a credible visual rule.

Analyze four demand vectors:

- Atmosphere: air state, light type, pressure, contrast, color temperature.
- Emotion: tension, sharpness, heaviness, softness, coldness, stickiness.
- Theme: what must be understood for the image to succeed.
- Situation: what materials, light, weather, and surface states are plausible here.

Then choose realism sources:

- light realism
- color arrangement
- material realism
- spatial realism
- force and feedback realism
- non-uniform, non-ideal details

### Object Priority

Do not assume the face or main character is always the highest priority.

Rank visible objects:

- A: success core, usually 7-10 texture parameters
- B: key support, usually 5-7 parameters
- C: environment completion, usually 3-5 parameters
- D: far filler, only general material, light, color, and spatial decay

Suggested description weight:

- A: 40-50%
- B: 25-30%
- C: 15-20%
- D: 5-10%

Bind texture to position. Do not write “realistic stone, realistic clouds, realistic clothing.” Write the lower foreground altar edge, the upper-right cloud mass blocking light, the mid-lower robe sleeve being lifted by updraft.

### Material Formula

`material base -> surface state -> dirt/damage source -> reflection type -> worn edge -> contact feedback -> inherited state`

Avoid:

- all objects equally wet, bright, dirty, or detailed
- metal all mirror-like
- leather like plastic
- cloth like rubber
- clouds as flat background
- water as pure mirror
- far background with macro detail
- texture priority disconnected from story priority

## Style and Artist Anchors

Use artists and directors as parameter sources, not as imitation labels.

Procedure:

1. Select at most three anchors.
2. Main anchor controls overall spirit and spatial structure.
3. Support anchor controls light, color, or material.
4. Detail anchor controls local rhythm, divine texture, speed, dream quality, or ink quality.
5. Compress into an 80-150 character front style anchor.
6. Do not let the style anchor replace action, unit, frame, or physics.

Examples of compatible uses:

- Divine spectacle: El Greco, Gustave Moreau, Wu Daozi, William Blake, Rothko.
- Wuxia/xianxia mountain pressure: Fan Kuan, Guo Xi, Li Tang, Ma Yuan, Fu Baoshi, Friedrich.
- Close action, blades, hands: Caravaggio, Ribera, Rembrandt, Degas, Goya.
- Wasteland industrial: Courbet, Daumier, Goya, Huang Binhong, Bacon.
- Modern urban supernatural: Caillebotte, Manet, Kirchner, Vermeer, Magritte.
- Dream or psychic space: Redon, Magritte, Dali, Chagall, Klee.
- Giant/doom pressure: Friedrich, Turner, Fan Kuan, Gericault, Fu Baoshi.

Avoid conflicting anchor groups unless the user intentionally wants dissonance. Strong chiaroscuro, impressionist air, and geometric abstraction can fight for control if all are made primary.

## Static Prompt Template

Use or adapt:

```text
【前置气质锚点】
80-150 字，定义光影、色彩、质感、情绪和禁止倾向。

【画面总述】
16:9 横版 / 竖版 / 正方形，一张承担“...”功能的关键帧。重点不是...而是...

【剧情功能锁定】
本画面的叙事目的：...

【正常动作系统】
动作阶段、支点、重心、握持方式、接触点、发力方向、可执行方式。

【单位关系锁定】
独立/连接/嵌套/复合整体/因果关联/遮挡关系。

【主体方位】
主体位于画幅...，朝向...，关键肢体/道具位于...

【机位方位】
机位相对主体...，高度...，景别...，焦段感...，目的...

【景深层级】
前景：...；中景：...；后景：...

【动作与物理反馈】
路径、接触、反作用、材质反馈、残留、尾状态。

【角色/道具/环境细节】
外貌、服装、武器、材质、表面状态、环境构件。

【画面质感】
光影、色彩、摄影感、空气、颗粒、质感限制。

【负面约束】
禁止...

【核心冻结状态】
画面冻结在...的瞬间。
```

## Preflight Checklist

- Is the image function clear?
- Is the action state physically executable?
- Are unit relations locked?
- Are frame coordinates concrete?
- Is the camera relative to the subject?
- Are foreground/midground/background distinct?
- Does every effect have a source?
- Are style anchors compatible and limited?
- Are negative constraints targeted to real failure risk?
- Does the frozen moment preserve the exact intended state?
