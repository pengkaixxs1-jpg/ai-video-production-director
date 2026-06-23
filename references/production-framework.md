# Production Framework

Use this reference for general AI video work, complex shot design, script-to-prompt translation, and project-level prompt systems.

## Why Parameters

AI video failures often come from handing abstract words directly to the model: realistic, oppressive, cinematic, heavy, fast, cold, dangerous, layered performance. The model averages those words into familiar templates. Parameterization turns professional intuition into visible decisions.

Four principles:

1. **Function before beauty.** A shot parameter exists because the shot has a task.
2. **Grouped parameters.** Heavy is not one word; it may require low camera, low center of gravity, low-frequency sound, slow startup, contact feedback, structural aftershock, and ground deformation.
3. **Bounded parameters.** High contrast can create pressure but can also lose faces; motion blur can show speed but can erase object identity.
4. **Frame first.** Every parameter must eventually become frame coordinates, depth layers, visible contact, sound source, or inherited state.

## Ten Modules

Choose three to five main modules per shot.

| Module | Responsibility | Trigger |
| --- | --- | --- |
| A Frame and composition | Subject position, depth, scale, obstruction, visual weight | Always first |
| B Camera | Relative camera, height, shot size, lens feel, movement, stability | Camera language or camera drift risk |
| C Light, color, air | Main light, contrast, color temperature, reflections, haze, particles | Realism, pressure, spatial depth |
| D Material and makeup | Skin, fabric, metal, dirt, blood, water, scratches, source and inheritance | Plastic look, mannequin look, clean studio look |
| E Performance and physiology | Eyes, breath, shoulders, fingers, weight, pain, emotional leakage | Emotion, injury, control, exhaustion |
| F Action and body mechanics | Support point, center of gravity, path, contact, reaction, recovery | Fighting, falling, rising, chasing, injury |
| G VFX and prop physics | Source, path, medium, object affected, speed, boundary, residue | Smoke, steam, sparks, water, wire, flying object |
| H Sound and dialogue | Source, direction, material, intensity, reverb, speech capacity | Space, weight, action causality, silence |
| I Continuity and editability | Opening/tail states, axis, focus chain, sound bridge, cut point | Multi-shot segments or review |
| J Model risk blocking | Explicit locks, negative constraints, likely hallucinations | Every final prompt |

## Module Notes

### A Frame and Composition

Start with the subject's frame position, not the story explanation. Use left/right/up/down plus foreground/midground/background.

Parameters:

- Subject 2D position: left upper, center lower, right lower, etc.
- Depth layer: near foreground, foreground, near midground, midground, background, far background.
- Frame share: under 10%, 10-30%, 30-60%, over 60%.
- Obstruction: none, partial, foreground cut, swallowed by shadow, edge cropping.
- Escape visibility: open, limited, blocked, completely sealed.
- Visual weight: highlight, contrast, dark mass, color accent, moving body.

Composition visualizes power. A blocked back path, low position, and foreground obstruction can say more about oppression than a line of explanation.

### B Camera

Always define the camera relative to the subject.

Parameters:

- Relative position: front, front-side, side, back, back-side, ground-level, overhead.
- Height: ground, knee, waist, chest, eye, high.
- Shot size: close-up, close shot, medium close, medium, full, wide.
- Lens feel: wide, normal, medium telephoto, long.
- Movement: fixed, slight push, follow, lateral slide, pan, low push, high-speed follow.
- Stability: locked, slight handheld, visible handheld, unstable pursuit, high-speed blur.

Movement needs a trigger: eye shift, prop flight, foot entering water, mechanical reveal, or sound source. Ban unmotivated orbit, zoom, and angle switching.

### C Light, Color, Air

Realism comes from light source logic, not from the word cinematic.

Parameters:

- Main light direction: front, side, top, back, side-back, gap leakage.
- Contrast: soft 2:1, realistic 4:1, hard 8:1, nearly black 12:1.
- Color temperature: cold white, blue gray, tungsten warm, fire orange, mixed dirty color.
- Reflection source: water, metal, glass, wet leather, blood, oil film.
- Air medium: dust, steam, cold fog, humidity, smoke, heat shimmer.
- Color accents: dark blood, blue electric arc, rust brown, brass edge, weak crystal glow.

Every local color should have function. Do not let blue electricity become a global filter or a stable magic weapon unless the setting demands it.

### D Material and Makeup

Material realism comes from source, non-uniformity, and inheritance.

Parameters:

- Material entropy: clean, lightly worn, heavily worn, oily rust, broken mix.
- Wetness: dry, damp, water film, soaked, dripping.
- Dirt source: fall, blast, splash, grip, wall scrape, machine oil.
- Skin state: sweat sheen, ash, mud spots, abrasion, blood trace, exhausted pallor.
- Clothing state: folds, tear, frayed edge, wet weight, clinging, broken strap.
- Metal state: oxidized, rusted, scratched, oily, condensed water, fresh cut.

Separate old marks from new marks. Old marks are darker and duller; new marks are wet, directional, and more specific.

### E Performance and Physiology

Emotion must enter the body.

Parameters:

- Eye focus: locked, avoiding, unfocused, refocusing, beyond camera.
- Breath: stable, shortened, urgent, broken, wet-heavy, low growl.
- Shoulder/neck: relaxed, tense, sunk, rigid, twitching.
- Fingers: open, clenched, trembling, unable to support, instinctively curling.
- Weight: stable, slight sway, slipping, kneeling, forcing recovery.
- Voice control: silent, short sentence, low voice, suppressing pain, coughing out.

Use the sequence control -> leakage -> spread -> suppression or failure. A cold authority figure often acts less, speaks lower, and leaves more silence.

### F Action and Body Mechanics

Actions need support, path, contact, reaction, and result.

Parameters:

- Support point: foot, knee, right hand, wrist, wall, pipe, prop.
- Center of gravity: centered, forward, backward, side-biased, losing balance, recovering.
- Force path: lift, press down, sweep, drag, ram, recoil.
- Contact point: fist, mechanical forearm, shoulder, palm, boot, prop edge.
- Reaction: shock to wrist, slip, bounce, debris, water spread, posture change.
- Aftermath: breath, pause, numb hand, fabric tear, ground mark.

Do not write only successful actions. Failed actions often create credibility and set up later reversals.

### G VFX and Prop Physics

Use source -> path -> medium -> affected object -> feedback -> residue.

Parameters:

- Source: broken pipe, mechanical shoulder, blade edge, puddle, guide rail, impact point.
- Path: direct spray, ground-hugging, arc, curl, thrown off, lateral spread.
- Medium: air, shallow water, oil film, metal, fabric, glass, steam.
- Speed: slow, short, fast, sudden stop, burst then decay.
- Scale: point, local, half body, corridor section, full space.
- Residue: ripple, blood trace, scorch, lingering fog, dying spark, object stop point.

Local elements must not become global conditions by accident.

### H Sound and Dialogue

Sound is a second spatial system.

Parameters:

- Action sound: water step, metal impact, cloth scrape, winch spin, glass click.
- Space sound: narrow alley echo, distant dripping, machine hum, broken pipe hiss.
- Physiological sound: breath, cough, pain gasp, swallow, low growl.
- Mechanical sound: gear bite, valve exhaust, tension arm vibration, thermal creak.
- Dialogue: speed, volume, gaps, broken phrasing, lowered register.
- Sound bridge: cross-shot continuation, early entry, tail residue.

Dialogue capacity follows physiology. A badly injured character cannot deliver long clean exposition.

### I Continuity and Editability

Each shot must be cuttable.

Parameters:

- Opening/tail state: position, posture, prop, wound, light source, sound, environmental damage.
- Axis: advance, retreat, gaze, prop flight, attack direction.
- Focus chain: hand -> weapon -> wire -> platform -> boot -> authority figure.
- Sound bridge: wire sound, mechanical hum, breath, dripping.
- Information density: low, medium, high, settling.
- Cut trigger: action completion, sound landing, gaze shift, contact, pause.

If a shot is beautiful but cannot pass focus or state to the next shot, it breaks the sequence.

### J Model Risk Blocking

Final prompts should contain targeted locks:

- frame axis and camera movement limits
- identity/injury/equipment locks
- prop existence and access locks
- VFX source and scale locks
- material inheritance locks
- no unmotivated angle switching, no restored wounds, no new props, no globalized effects

## Five-Step Translation From Script

1. Find state change: who changes from what to what?
2. Find visible/audible evidence: what proves the change?
3. Select main modules: which parameters carry the change?
4. Control frame and depth: where is each evidence item?
5. Write tail state: what does the next shot inherit?

This prevents two failures: too much story explanation without evidence, and rich image detail with no reason to exist.

## Compact Parameter Sheet

Use this before expanding:

| Field | Fill |
| --- | --- |
| Subject position | Frame coordinates, depth, share, facing, movement |
| Relative camera | Position, height, shot size, lens feel, movement |
| Fore/mid/background | Obstruction, subject, anchor, light source |
| Light/color | Main light, contrast, temperature, reflection, air, accent |
| Material/makeup | Clothing, skin, metal, dirt, wetness, source, inheritance |
| Performance/body | Eyes, breath, shoulders, fingers, weight, voice |
| Action/physics | Support, path, contact, reaction, success/failure result |
| VFX/props | Source, path, medium, speed, scale, residue |
| Sound | Action, space, physiology, machine, dialogue, bridge |
| Tail state | Position, posture, prop, wound, environment, sound |
| Negative locks | Three to five likely generation failures |

Execution mantra:

Lock frame position first. Define camera relative to subject. Give foreground, midground, and background before fine detail. Pick a shot purpose before selecting modules. Write support, path, contact, and feedback before emotion and atmosphere. Ensure tail state can cut to the next shot. Turn all abstract adjectives into visible, audible, inheritable evidence.
