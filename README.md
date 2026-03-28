<p align="center">
<img width="1280" height="640" alt="TN-LevelWalkthrough-LDGameJam10" src="https://github.com/user-attachments/assets/5ff13b6b-3f58-48dc-9d35-1c1f32a9cdb5" />
</p>

# Glass Smile: Stealth-Horror Level Design Breakdown
![Unreal Engine](https://img.shields.io/badge/Unreal_Engine-5.6+-black?logo=unrealengine)
![Role](https://img.shields.io/badge/Role-Level_Designer-blue)
![Project Type](https://img.shields.io/badge/Project-Jam_Prototype-brightgreen)
![Status](https://img.shields.io/badge/Status-Completed-success)

This is a short 3D first-person atmospheric horror level created for a Level Design Jam 10 by Steve Lee within one month. The player must find a way out of a haunted Japanese tea house. The focus is on spatial pacing, enemy placement, and building tension through level structure.

## About Me & This Repository
Whatsup homie! I'm Melinn 👋, your favorite game designer based in Vancouver, BC. I created this repository as a portfolio deep-dive. While playing a game shows the final result, I wanted a place to openly share my source files and document the specific design philosophies and problem-solving that went into building this tension-driven experience. 

## What is Orthogonal Design?
At its core, this concept originates from **Orthogonal Experimental Design**, a statistical methodology used to analyze multiple independent variables without them interfering with each other.

In game design, orthogonal design means creating a different kind of encounter, rather than just changing a quantitative value. Instead of scaling difficulty linearly (like just giving an enemy more health or making them walk faster), orthogonal design challenges the player on completely different mechanical axes. This forces the player to constantly adapt and change their strategy depending on the specific threat in the room.

The 3 key principles of this methodology applied to encounter design are:
- **Orthogonality (Independence)**: Enemy mechanics do not overlap. Each enemy tests a completely different player skill or interaction.
- **Balance**: Each factor is utilized at different levels, ensuring the distinct mechanics have room to breathe without overwhelming the player.
- **Efficiency**: Maximizing the depth of the player's tactical decisions using a minimal, highly intentional roster of enemies.

## How I executed it
Because this was a one-month horror game jam, I needed to keep the scope tight. I broke the enemy encounters down into **3 distinct behavioral axes: The Psychological Axis, The Spatial Axis, and The Attention Axis.** By ensuring these variables did not overlap, each enemy demands a completely different cognitive and mechanical response from the player.

### The Encounter

- **Mimamori Onna (The Psychological Axis)**
  - **Mechanic**: Constant observation with zero lethality. *(She's watching you)*
  - **Orthogonal Function**: She decouples visual threat from the mechanical failure state. Because she causes **no harm**, she tests the player's emotional regulation, forcing them to ignore a highly visible false threat and preserve their cognitive load for actual dangers.

- **Oi Onna (The Spatial Axis)**
  - **Mechanic**: Autonomous patrol with active lethality. *(She's patroling and hunting)*
  - **Orthogonal Function**: She acts as the traditional threat and operating entirely on spatial navigation. Her presence tests positioning and movement. The required counter-play is strict evasion and **breaking line-of-sight**.

- **Misume Onna (The Attention Axis)**
  - **Mechanic**: Conditional lethality dependent on the player's camera vector. *(She's hunting when you're not looking at her)*
  - **Orthogonal Function**: She operates on the axis of player attention. Unlike Oi Onna, the required counter-play for Misume Onna is **maintaining direct line-of-sight.**

## My Design Philosophy
While academic "Orthogonal Design" suggests units should be 100% independent, I found that in a one-month jam, the most effective approach was **a hybrid of Orthogonality and Differentiation by Degrees.**

> [!TIP]
**"Differentiation by degrees"** occurs when units differ in intensity or value (speed, health, detection range). While most games are rarely 100% orthogonal, what matters most is ensuring the player has tactically meaningful decisions.

### My Approach:
- **True Orthogonality**: Mimamori (No harm) vs. Oi (Harm). These are binary opposites. Their purpose and the player's emotional response to them do not overlap.
- **Differentiation by Degrees**: Misume Onna acts as a bridge. She introduces a conditional threat that depends on a shared variable (player attention), requiring the player to manage their focus as a resource.

## Level Design: Encounter Breakdown
Each enemy is mechanically simple by design! The complexity arises not from the AI code, but from intentional level placement. By combining these simple behaviors in specific "Beats," I created emergent counterplays where the player is forced to juggle conflicting rulesets simultaneously.

### Beat 04
![Beat6_Showcase](https://github.com/user-attachments/assets/e2b6b712-7aa8-4726-9f53-60b7587de8fe)

I introduced two Oi Onna with staggered paths and timing. The player has to wait for the first to pass, then gets chased by the second. It creates a panic moment through pacing alone.

### Beat 06
![gifgit](https://github.com/user-attachments/assets/6cb7fc4f-5d8f-437d-b293-7803bc3c0bb1)

I combined an Oi Onna and a Misume Onna. The player has to keep an eye on Misume to stay safe, while timing their movement to avoid Oi Onna. Later, they’ll run into Oi Onna again. It forces them to think about timing and where they're looking at the same time. That moment came from the placement. That’s emergent gameplay.

### Beat 08
![Best8_Showcase](https://github.com/user-attachments/assets/2afa5c6b-334b-4400-9d49-d3b91cb07cae)

I used 3 Misume Onna. Instead of constant threat, I used placement to create rhythm. The player must stare down the first one, let the other two walk toward them, then sprint through the gap, and quickly turn around to freeze them. Moments like this come from pacing the encounter like a sequence. It became a tense moment with tight timing and a satisfying challenge.


<img width="1920" height="1080" alt="Level Beat" src="https://github.com/user-attachments/assets/ea0889f1-d1eb-4160-b8d0-a7efba9a69ce" />

> <sub> **Watch full walk through video by [Queen faith official](https://www.youtube.com/@queenfaithofficial9309) here: https://www.youtube.com/watch?v=aT830qQ-hgY** <sub>

## Key Takeaways
Orthogonal design is indeed theoretical framework, but its success depends entirely on the context it lives in. This project served as a deep dive into how high-level systems theory translates into actual player experience.
- **Systems + Context**: Orthogonal design alone doesn't create "fun." The true power of simple, decoupled mechanics is only realized when combined with intentional encounter pacing, spatial layout, and player-centric iteration.
- **Simplicity is Scalable**: I learned that even the most basic mechanics feel more impactful when they are mechanically distinct. It allows for a high 'depth-to-complexity' ratio, keeping the project scope manageable without sacrificing engagement.
- **The Power of the Pivot**: Some initial orthogonal combinations felt mathematically correct on paper but weren't playfully right. Iterating based on tester feedback was the only way to find the actual rhythm.

> [!IMPORTANT]
**Keep orthogonal design in your toolkit, but never let theory override the "feel."** You won’t know if your different kinds of encounters actually work until you put them in front of a player. Keep experimenting! That’s how fun experiences are made!!

---

<p align="center">
  <a href="https://mightymelinn.itch.io/glass-smile-level-design-jam-10">🕹️ Play the Prototype</a> | 
  <a href="https://sites.google.com/view/melinnportfolio/home">🎨 Check out my portfolio</a> | 
  <a href="https://www.linkedin.com/in/melinn/">✉️ Connect on LinkedIn</a>
</p>


<p align="center">
<sub> Copyright (c) 2026 Melinn. All rights reserved. Developed for portfolio purposes. <sub>
</p>
