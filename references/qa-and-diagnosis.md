# QA and Diagnosis

Use this reference for reviewing prompts, storyboards, generated images/videos, failed outputs, and skill iterations.

## Scoring

Score out of 100:

| Item | Points | Check |
| --- | ---: | --- |
| Spatial continuity | 20 | subject position, axis, escape path, foreground/background stability |
| Physical causality | 15 | support, contact, reaction, residue |
| Light/material realism | 15 | light source, contrast, color, reflections, material response |
| Performance credibility | 10 | emotion through body, breath, gaze, control/leakage |
| Action readability | 10 | speed, path, target, stop point |
| Sound anchors | 10 | source, direction, material, reverb, bridge |
| Editability | 10 | focus chain, sound bridge, opening/tail state |
| Model blocking | 10 | targeted locks for likely hallucinations |

Below 80, rewrite before final delivery. Below 60, re-diagnose the task instead of patching words.

## Failure Patch Template

```text
失败现象：
参数归因：
缺失变量：
修正变量：
负面封堵：
下一版测试点：
```

## Common Failures and Counter-Parameters

### “Not cinematic”

Usually too vague. Diagnose:

- Is there a main light source?
- Is contrast controlled?
- Are foreground/midground/background separate?
- Is camera position relative to subject?
- Is there a focus chain?
- Is there a reason for lens/motion?

Patch with concrete light, camera, depth, and focus evidence.

### “Not realistic”

Diagnose:

- Are material sources visible?
- Does wetness/dirt/damage have cause?
- Are all objects equally detailed?
- Are far objects over-described?
- Does force create expected feedback?
- Does the next shot inherit traces?

Patch with material base, surface state, source, reflection, contact feedback, and inherited state.

### “Action floats”

Diagnose:

- missing support point
- missing center of gravity
- missing contact point
- no attacker reaction
- no defender/environment feedback
- injury ignored

Patch with action chain nodes and body limits.

### “Cut feels random”

Diagnose:

- previous shot has no signal
- signal debt is abandoned
- no operator chosen
- no audience change
- style transition overrides continuity

Patch with previous tail signal, attention expectation, cut operator, and audience information/emotion/action change.

### “Prop appears from nowhere”

Diagnose:

- missing pre-existence
- unclear position
- access path impossible
- state jumps
- fake setup too obvious

Patch with body, position, trace, route.

### “Character drifts”

Diagnose:

- reference treated as inspiration instead of identity anchor
- too many re-descriptions of face
- action overrides injury
- panel treated as independent poster
- clothing/dirt not inherited

Patch with identity/state/performance layers and priority locks.

### “Mechanical object mutates”

Diagnose:

- structure not partitioned
- joint count not locked
- action written as visual result, not mechanical path
- speed/effects hide structure

Patch with silhouette, joints, linkage, support, trajectory, tail state.

### “VFX swallows scene”

Diagnose:

- no source
- no boundary
- local element became global
- no medium/path
- no residue duration
- effect scale mismatches shot size

Patch with source, path, medium, affected object, scale, decay, residue.

### “Dialogue breaks body state”

Diagnose:

- injured character speaks too much
- authority character over-emotes
- speech has no spatial ownership
- no breath or pause logic

Patch with speech capacity, volume, speed, breaks, body state, and space ownership.

## Red Lines

- One shot carries too many main ideas.
- Abstract emotion has no body evidence.
- Style words replace physical logic.
- Effects have no source.
- Contact has no contact point.
- Impact has no reaction.
- Environment resets without explanation.
- Previous signal is ignored.
- Axis breaks without design and repair.
- Props are used before existing.
- Identity, injury, equipment, or mechanical structure changes to make action easy.

## Review Order

1. What is the task function?
2. What is the main evidence?
3. Is frame position concrete?
4. Are units separated correctly?
5. Does action have support/contact/reaction?
6. Do light/material details have sources?
7. Does sound prove space, action, or body?
8. Is the shot cuttable to the next?
9. Are negative constraints targeted?
10. What should be stored as a future project rule?

## Patch Deposition

When a failure repeats, turn it into a reusable patch:

- name the failure
- define when it triggers
- describe root cause
- list required variables
- list red lines
- give a compact mountable text
- add it to the appropriate reference or skill

Do not add every one-off preference to the skill. Only add rules that improve future generalization.
