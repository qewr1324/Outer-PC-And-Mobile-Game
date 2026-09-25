<style>

.counter {
   opacity: 100%;

   &:hover {
      opacity: 90%;
   }
}

</style>

<p align="center" >
   <img src="https://img.shields.io/badge/VSCode-1.139.1-abcdef?style=flat">
   <img src="https://img.shields.io/badge/.NET%208-512BD4?logo=dotnet&logoColor=fff">
   <img src="https://img.shields.io/badge/Unity%206.0-black?style=flat&logo=unity">
   <img src="https://custom-icon-badges.demolab.com/badge/C%23-%23239120.svg?logo=cshrp&logoColor=white">
   <img src="https://img.shields.io/badge/Apache%20Licence-2.0-0091ea?style=flat&labelColor=0071b7">
</p>

# Outer

<div align="center">

<img src="./Example/Example - 0.webp" style="border-radius: 16px;" class="counter" />

</div>

> 🧃 A tiny lone figure in a simple spacesuit, standing in a vast dark entrance chamber.

**Outer** is a sci-fi mystery game about a signal technician sent to an abandoned station at the edge of the system. What he finds isn't just silence — it's something that watches, mimics, and waits.

This repo is home to two things: the **C# minifier package** that powers part of the project's toolchain, and the **design docs** for the game itself — world, creatures, structure, and the puzzles that hold it all together.

---

## 🧬 Logline

<div align="center">

<img src="./Example/Example - 1.webp" style="border-radius: 16px;" class="counter" />

</div>

A signal technician is sent to a derelict space station to find out why communications went dark. What he finds is not silence — but creatures that first seem curious, then helpful, then hungry. He has to uncover the truth and escape before he becomes part of them.

---

## 🌌 The World: Outer

<div align="center">

<img src="./Example/Example - 2.webp" style="border-radius: 16px;" class="counter" />

</div>

Outer is a massive structure orbiting a dead star — part research station, part asteroid mine, part alien temple. Years ago, a team of scientists picked up a signal from deep space. They thought it was a message from a distant civilization.

It was a trap.

The station is built in three layers:

| Layer | Description |
| --- | --- |
| **Shell** | Industrial corridors, sealed hatches, flickering lights. Where humans used to live. |
| **Biology** | Labs, hydroponic farms, and the first signs of growth. The walls breathe. |
| **Nest** | Organic, dark, alive. Physics here doesn't work the same way. |

---

## 🔘 The Creatures: The Chorus

<div align="center">

<img src="./Example/Example - 3.webp" style="border-radius: 16px;" class="counter" />

</div>

They don't start as monsters. They *become* monsters — slowly, in three stages.

**1. Curious & Beautiful**
Shadows in the distance. Whispers. Faint singing. They open doors for you, light paths. You think they're survivors.

**2. Mysterious & Unpredictable**
They help, then block your way. You realize they're mimicking human voices to pull you closer. The first body shows up.

**3. Hunter & Malevolent**
They're a collective mind feeding on neural energy. You're not a guest — you're food. Or a host. They stop pretending.

They're not *evil* in a moral sense. But from where you're standing, they're the thing trying to kill you. That grayness is what makes the ending land.

---

## 📖 Three-Act Structure

<div align="center">

<img src="./Example/Example - 6.webp" style="border-radius: 16px 16px 5px 5px;" class="counter" />

</div>

**Act I — Silence**
You arrive. Nothing moves. Puzzles are simple — lights, hatches, gravity. Crew logs say *"they're not dangerous, just curious."* At the end, you see one up close. It doesn't touch you. It leaves.

<div align="center">

<img src="./Example/Example - 8.webp" style="border-radius: 5px" class="counter" />

</div>

**Act II — The Turn**
They show up more. Some attack. Puzzles get meaner — you avoid them, redirect their sound, use them. A new log: *"They mimic sounds. Don't answer the voice asking for help."* You find a body surrounded by them. You enter the nest. The way back closes.

<div align="center">

<img src="./Example/Example - 4.webp" style="border-radius: 5px 5px 16px 16px;" class="counter" />

</div>

**Act III — The Nest**
Walls made of creatures. Breathing rooms. Puzzles built on light, sound, and gravity — they hate light, they follow sound, they swim in zero-G. The truth: the signal was bait. Outer is a farm. Ending is yours to pick — destroy the core and run, or merge with it and become something else. Either way, you'll never know how many other stations are still waiting.

---

## 🧩 Puzzles as Storytelling

<div align="center">

<img src="./Example/Example - 7.webp" style="border-radius: 16px;" class="counter" />

</div>

Like Inside, the puzzles aren't filler — they *say* things.

- **Light** — creatures hate it. Route light to carve a safe path, but too much and they snap.
- **Sound** — make noise elsewhere to lure them away. Later, they learn *your* voice and use it against you.
- **Gravity** — rotating sections flip everything. You solve in 3D. They hunt in 3D.
- **Organic** — use their fluids as a conductor. Faster, but it calls them. Speed or safety?

---

## 🎥 Why a Distant Isometric Camera

<div align="center">

<img src="./Example/Example - 21.webp" style="border-radius: 16px;" class="counter" />

</div>

- You look small. Outer looks huge.
- You see multiple rooms at once — connections become visible.
- Seeing something move *far away* and not knowing where it's going is worse than seeing it up close.
- Cheaper to render — detail matters less when the focus is light, shadow, and silhouette.

---

## 🛠️ Unity Notes

- **Render pipeline:** URP for mobile + desktop. HDRP only if the team is solid and PC is the target.
- **Shaders:** Monochrome, high contrast, volumetric fog, bloom, vignette — built in Shader Graph.
- **Camera:** Cinemachine, isometric mode, locked angle, auto-fade on blockers.
- **Platforms:** Linux/BSD builds work but test them. Mobile needs LOD + baked lighting.
- **Puzzles:** Event-driven scripts + state machines, so each puzzle stays modular and combinable.

---

## 🏷️ Title Ideas

- **Outer: The Chorus**
- **Outer: Silence**
- **Outer: The Lure**

---

## 🎯 The Point

Curious → Guide → Hunter. That's the arc. Tie every puzzle to light, sound, gravity, or flesh. Keep the ending gray. Don't explain too much. Let the silence do the work.
