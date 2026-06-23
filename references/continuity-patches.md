# Continuity Patches

Use this reference for multi-shot continuity, prop/hazard pre-existence, character anti-drift, injury/equipment inheritance, and mechanical structure conservation.

## Patch 1: Pre-Existence Chain

Rule:

`先存在，后使用；先可见/可感/可推知，后成为剧情作用点。`

Anything later used, affecting action, changing situation, or carrying physical feedback must have prior body, position, trace, and access path.

Objects include:

- props: pipe, brick, crystal, broken blade, gas tank, rope, machinery part
- environment: wall corner, low pipe, broken pipe, junk pile, doorway, puddle, slope, crack, step
- hazards: electricity, steam, conductive water, loose board, collapse point
- character state objects: bag, strap, wound, dropped object, held object, foot-side object
- intervention units: platform, authority figure, cable, bottle, light, shadow, sound source

### Core Rules

1. **Later-use object must have earlier root.**
   - Explicit: directly visible.
   - Semi-explicit: visible at edge, depth, or behind obstruction.
   - Trace-first: sound, reflection, steam, silhouette, shadow, disturbance.

2. **Earlier setup must be preserved until payoff.**
   - Establish object.
   - Preserve state or relation.
   - Let character contact, use, or suffer from it.

3. **Access path must be physically possible.**
   - How far is it?
   - Can the character reach it?
   - What posture allows contact?
   - What blocks the path?
   - Do injuries and center of gravity permit it?

### Four Levels

1. Existence: the audience can know it is there.
2. Spatial lock: relative position to character/environment is clear.
3. State preservation: it does not jump, clean itself, or change function randomly.
4. Functional payoff: later use matches established state.

### Hidden Check Column

For every shot, ask:

1. Does this shot contain anything used later?
2. Does it have a clear position?
3. Does the character have contact possibility?
4. Will it actually be used? If not, do not overemphasize it.

Mantra:

`后镜能用之物，前镜必有其身、其位、其迹、其路。`

## Patch 2: Character Anti-Drift

Use for storyboard grids, continuous keyframes, identity references, multi-panel images, and long shot sequences.

Core task: keep the same character in the same continuous action chain, not six independent posters.

### Information Layers

1. **Identity layer**: face shape, feature proportions, age, gender temperament, hair outline, skin state, major scars. Highest priority.
2. **State layer**: current injury, cough/blood, usable limbs, hand injury, equipment, held object, dirt, wetness, damage. Must inherit current story node.
3. **Performance layer**: action, gaze, emotion intensity, composition, light pressure. May change, but cannot invade the first two layers.

Priority:

`identity > injury > equipment > action > composition > style`

### Rules

- Treat reference images as identity anchors, not loose inspiration.
- One character should have one main identity anchor; add a state anchor if needed.
- Multi-panel grids are state chains. Panel 2 inherits panel 1 tail state; panel 3 inherits panel 2 tail state.
- Each panel gets one main change and at most two secondary changes.
- For reference-defined details, write locks rather than re-invented portrait descriptions.
- Critical injuries must be written as prohibitions: cannot lift left arm, cannot fully support with injured palm, cannot suddenly move smoothly.
- Clothing, dirt, wetness, and damage are continuity, not decoration.

### Anti-Drift Checklist

- Is the face still the same person?
- Are facial proportions, eye distance, nose bridge, mouth, and age stable?
- Is hairstyle length, flow, wetness, and fringe stable?
- Are injuries preserved and in correct locations?
- Is equipment present/absent according to current story phase?
- Are clothing length, layer, straps, tear locations, and boots stable?
- Is the character still in the same story node?

Default negative constraints:

- no face drift
- no age drift
- no hairstyle drift
- no clothing-structure drift
- no injury loss
- no unexplained equipment appearance/disappearance
- no restoring damaged limbs to make the action easier
- no treating panels as unrelated illustrations

## Patch 3: Mechanical Structure Conservation

Use for mechanical arms, prosthetics, platforms, equipment, wires, mechanisms, evidence devices, industrial props, and complex tools.

Core:

`先守住它是什么，再允许它怎么动。`

### Principles

1. A complex machine is a structure, not a visual impression.
2. Motion cannot sacrifice structure.
3. Unit independence and unit relation must both hold.

Mechanical action must be achieved through:

- joint rotation
- torso or base drive
- support point changes
- center of gravity transfer
- connection linkage

Do not use:

- limb length change
- shell rewrite
- endpoint reshaping
- extra joints
- fixed parts changing shape for convenience

### Structure Partition

For each complex machine, split:

- connection mount
- upper segment shell
- hinge/joint
- fore segment shell
- rotating wrist/connector
- end effector
- pipes/cables/auxiliary parts
- material layer and weight

For each action, specify:

- which segment moves
- which segment is carried
- which segment remains stable
- which segment bears force

### Mechanical Action Solver

Do not write only “sweep, smash, block.” Fill:

1. starting posture
2. force source: shoulder socket, torso, base, motor, recoil
3. main moving segment
4. support point
5. motion path through the frame
6. tail state and environmental feedback

Priority:

`outer silhouette > joint logic > body/base linkage > motion path > speed feeling > effects`

Effects such as electricity, steam, and sparks are auxiliary and must not hide structure.

### Mechanical Checklist

- Is the outer silhouette stable?
- Are joint count and position stable?
- Is the end effector stable?
- Is motion achieved by joints and linkage?
- Did the model change shape to make motion work?
- Is material and weight preserved?

Default negative constraints:

- no length changes
- no joint count changes
- no endpoint redesign
- no turning platform into humanoid mech
- no direct clipping through containment bottle or glass
- no mechanical arm flying independently while body freezes
- no speed blur that erases structure identity
