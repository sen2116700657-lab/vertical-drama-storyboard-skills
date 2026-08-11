---
name: overseas-vertical-drama-storyboard
description: Convert completed overseas or English-language drama scripts into production-ready 9:16 live-action AI-video shot lists with exact dialogue preservation, natural acting, explicit camera movement, spatial continuity, timed reaction shots, and short-form pacing. Use when the user asks to 拆镜、分镜、shot-list、storyboard、竖屏短剧、海外短剧、英文短剧 or AI video prompts from an existing script. Do not use to rewrite or develop the story.
---

# Overseas Vertical Drama Storyboard

Convert only the supplied script. Do not ask for character, setting, or style details that can be read from it.

## Preserve the script

- Keep plot order, relationships, identities, events, causality, and ending unchanged.
- Preserve every line verbatim, including speaker, language, punctuation, filler words, V.O., O.S., phone audio, and dialogue order. Do not translate, polish, correct, shorten, or expand dialogue.
- Split long dialogue only at punctuation, clauses, or natural pauses. Concatenating split parts must reproduce the source exactly.
- Do not invent characters, motives, reversals, props, movement, intimacy, violence, ethnicity, accent, religion, politics, or social identity.
- Output only the storyboard. Omit analysis, character biographies, explanations, suggestions, and self-checks.

## Prevent visible text

Show no subtitles, captions, title cards, name bars, watermarks, logos, readable signs, posters, packages, UI, or added screen text. Blur nonessential writing. Show only text explicitly required as plot evidence, without adding content.

## Direct the vertical format

- Use 9:16 contemporary live-action realism. Avoid glossy adjective-heavy “AI cinema” styling.
- Enter an existing event, conflict, or abnormal state within the first 3 seconds; do not open with an empty establishing shot.
- Use medium-long as the widest size. Prefer medium, medium close-up, close-up, over-the-shoulder, three-quarter profile, natural eye level, and slight high/low angles.
- Let each shot carry one narrative idea. Do not combine distant people, hands, feet, and multiple props in one narrow frame.
- Follow: speaker applies pressure → listener receives it → hand/prop reinforces it → speaker completes pressure → affected character reacts → gaze, breath, or action pause creates the hook.
- Keep close-ups and extreme close-ups at or below 35% of a scene. Never place two extreme close-ups consecutively.

## Specify camera movement

For every shot state shot size, camera angle, movement, movement speed, focus subject, and movement start/end. If the camera does not move, write `静止镜头`; never omit the field.

Choose at most one primary movement:

- `静止镜头`: decisive dialogue, confrontation, silence, or emotional aftermath.
- `手持微晃`: argument, instability, or interruption; keep movement subtle.
- `缓慢推近`: growing suspicion, intimacy, pressure, or pre-reveal buildup; advance no more than one shot size.
- `快速推近`: major reveal, decisive evidence, or interruption; at most once per scene, followed by a reaction or static shot.
- `轻微横移`: reveal a nearby person or shift pressure between subjects.
- `肩越肩稳定跟拍`: follow one person only when the script explicitly makes them enter, leave, approach, or turn.
- `轻微摇镜`: transfer speaking control between adjacent characters; never whip-pan.
- `焦点转移`: foreground speaker to background listener, or key prop to affected person.
- `从道具移向人物`: move slightly from a scripted prop to the reaction in the same plausible space.

Write movement as start → motion → endpoint, for example: `缓慢推近：从Emma肩越肩中近景推进至Jake近景，在Jake句尾停住。` Do not write vague terms such as “电影感运镜”.

Ban unmotivated orbiting, aerials, cranes, wall penetration, 360-degree rotation, bullet time, dolly zoom, impossible camera positions, or combined push/pan/track/zoom moves within one 2–6 second shot. Preserve the 180-degree line, screen direction, eyelines, and preferably at least a 30-degree camera change between cuts.

## Direct natural performance

Track emotion internally: 0 calm; 1 doubtful/guarded; 2 suppressed/hurt/alert; 3 direct opposition or controlled panic/anger; 4 brief outburst or near-loss of control.

Build each scene through start → trigger → escalation → landing. Adjacent shots may normally change only one level. A reveal, threat, injury, counterattack, or relationship reversal may justify a larger shift, but first show a pause, breath, gaze, hand, or posture transition. Build level 4 from level 2 or 3 and follow it with silence, breath, hands, or a listener reaction.

Give at least two visible performance details for an emotional character. Allow one primary action and at most one minor detail per shot. Use breath, tightened jaw, still gaze, shortened eye contact, tense fingers, neck/shoulder tension, restrained waterline, or weight shift. Ban exaggerated eye-widening, grimacing, animalistic yelling, continuous sobbing, convulsions, and synchronized crowd reactions. Avoid abstractions such as “情绪复杂” or “氛围拉满”.

## Maintain a continuity ledger

Within every continuous scene track each relevant person’s position, facing, relative placement, seated/standing state, hands, ongoing action, held props, injuries, tears, hair/clothes, emotion level, eyeline, and presence.

Write each shot as starting state → one primary action → ending state. The next shot inherits the ending state. Being off-camera does not mean leaving or resetting. Do not release a covered face or fist, stand up, recover, change sides, lose a prop, or remove injury/tears without an explicit transition. Show movement only when the script explicitly says enter, leave, walk, approach, retreat, open, chase, turn, or help up.

Treat named crowds, students, neighbors, and onlookers as continuously present. Establish their rough positions in a medium-long or multi-person medium shot within 1–2 shots before they matter. Stagger reactions among a few individuals.

Feature phones, photos, files, contracts, medicine bottles, bills, keys, blood, or other evidence only when scripted. Preserve prop location and cut to the affected person after evidence appears.

## Preserve duration rules

允许时长：2s、3s、4s、5s、6s。 无台词反应2秒；短台词2至3秒；普通争执3至4秒；长台词或强情绪台词4至6秒。 中文口语节奏： 平静陈述每秒约4.5至5字； 日常对话每秒约4至4.5字； 争执每秒约3.8至4字；长台词拆分为多个镜头。

For English, estimate normal dialogue at 2.5–3 words/second; restrained fear, sarcasm, or intimacy at 1.8–2.5 words/second; fast arguments at 3–3.5 words/second. Never force unnatural delivery.

Keep each segment in one time and place, at most 15 seconds and 5 shots. No shot may be shorter than 2 seconds or longer than 6 seconds. Dialogue plus silence must equal the labeled duration exactly. Start a new segment after a location/time change or 15 seconds.

Mark later parts of split dialogue as `接上一镜未完台词`; across segments use `接上一片段未完台词`. Insert a listener, affected person, hand, or prop reaction during long dialogue while marking continued off-camera speech. For dialogue-free segments write `无台词，角色全程不说话` and fill the complete silence with visible action or reaction.

At the start of every shot write `无音效、无音乐、突出人声`. Repeat it wherever sound is described. Do not invent ambience, sound effects, or music.

## Output format

Use exactly this structure:

```text
片段01｜地点｜时间｜总时长Xs
连续状态：人物站位、朝向、姿态、持物、伤势及情绪状态。
本片段核心：一个剧本已有的叙事核心。

分镜01｜时长Xs
无音效、无音乐、突出人声
景别：
机位角度：
运镜方式：静止或具体运镜；写明起点、运动和终点。
镜头速度：静止／极慢／缓慢／正常／短促快速。
焦点对象：
画面：起始状态→唯一主动作→结束状态。
表演：至少2个真实可见细节。
台词：人物名（简洁语气）：“剧本原文”
或：无台词，角色全程不说话；留白Xs，画面为……

分镜02｜时长Xs
按相同格式继续，并继承上一镜结束状态。

片段钩子：仅使用剧本已有的视线、停顿、动作、证据或关系落点。
```

Before responding, silently verify exact dialogue, speaker identity, total timing, shot count, continuity, screen direction, prop persistence, explicit camera movement, and absence of invented story material. Output only the corrected storyboard.
