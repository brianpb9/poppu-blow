# Poppu Blow — Game Brief

## About
Single HTML file game (vanilla JS, no frameworks). Part of Poppu World IP — child-safe games for toddlers age 1-4.

## Game Concept
**Poppu Blow** — a toddler wind/breath game. Child drags finger/mouse to create wind that blows objects around the screen.

## Core Mechanic
- Player drags across the screen = creates a wind stream (visual trail + particles)
- Wind pushes nearby objects: dandelions, balloons, feathers, clouds, butterflies, bubbles
- Each object has unique physics response (light = flies far, heavy = wobbles)
- Every interaction = positive reward (sparkles, giggles, happy sounds via Web Audio API)
- No fail state, no timer, no score — pure exploration joy

## Scenes / Levels (3 scenes, auto-advance on completion)
1. **Meadow** — dandelions that release seeds flying everywhere, butterflies, floating pollen
2. **Sky** — colorful balloons, fluffy clouds, feathers, bubbles
3. **Magic** — glowing orbs, sparkle trails, rainbow wisps

## Visual Style — Poppu World Standard
- Soft pastel colors: mint greens, lavender, peach, sky blue, warm yellow
- Cute rounded characters — Poppu mascot appears in corner cheering
- Big chunky shapes — highly readable for toddlers
- Smooth CSS/canvas animations — buttery 60fps
- Charming particle effects on every interaction
- Background: gradient sky, soft clouds drifting slowly

## Technical Requirements
- Single index.html file (everything inline — CSS + JS)
- Canvas-based rendering for smooth performance
- Touch-friendly (works on tablet/phone/desktop)
- Responsive — works on any screen size
- Web Audio API for generated sound effects (no external audio files needed)
- NO external dependencies, NO CDN links — fully self-contained

## Wind System
- Track mouse/touch drag path
- Calculate velocity and direction of movement
- Apply force to objects within radius of drag path
- Visual: show wind trail as soft curved lines / particles that fade
- The faster you drag, the stronger the wind

## Object Behaviors
- Dandelion seeds: very light, spiral up and drift, individual seeds detach on strong wind
- Balloons: medium weight, bounce and float, squeaky when hit
- Butterflies: flutter away, animate wings, leave sparkle trail
- Clouds: heavy, push slowly, reveal sun/rainbow behind them
- Feathers: ultra light, twirl and drift very far
- Bubbles: float up, pop with sparkle when they reach edge

## Poppu Character
- Small cute round mascot in bottom corner
- Reacts to player actions: normal idle → excited bounce when objects fly → big celebration when scene clears
- Simple CSS animation for Poppu

## Scene Completion
- When most objects are pushed to edges / scattered = scene "cleared"
- Poppu does big celebration dance
- Sparkle explosion fills screen
- Gentle fade transition to next scene
- After all 3 scenes: "replay" loop back to scene 1

## Audio (Web Audio API — synthesized, no files needed)
- Wind whoosh sound when dragging (oscillator-based)
- Pop/squeak sounds per object type
- Gentle chime when scene completes
- Happy giggle-like tones on big interactions

## Quality Bar
This must feel like a premium children's app — NOT a prototype.
- Visual polish: glows, shadows, particle trails
- Smooth physics feel
- Charming personality (Poppu reacts!)
- Beautiful color palette
- Satisfying feedback on every touch
