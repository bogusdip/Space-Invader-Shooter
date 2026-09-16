# Top-Down Space Shooter

<img width="720" height="406" alt="gameplay" src="https://github.com/user-attachments/assets/317c7d11-08bf-471f-88a6-3d68c8fdeded" />


A top-down space shooter prototype built with p5.js. The player ship uses acceleration-based WASD movement and fires mouse-aimed projectiles. Enemies use two distinct AI behaviors: one type orbits the player at a fixed range with staggered attack timing, and another uses a predictive-intercept calculation to aim ahead of the player's movement rather than just chasing their current position. Includes custom collision detection (line-circle intersection for projectile hits, circle-circle separation for enemy overlap).

**[Play it / view the code in the p5.js editor →](https://editor.p5js.org/lucas.airewele/sketches/XSWUq6prC)**

## Controls

| Action | Key |
|--------|-----|
| Move | WASD |
| Aim | Mouse |
| Fire | F |

## Features

- Acceleration-based player movement with mouse-aimed projectile firing
- "Orbiter" enemy type: circles the player at a fixed radius, with attack timing staggered evenly across the group so shots don't all fire at once
- "Charger" enemy type: uses a predictive-intercept calculation based on the player's velocity to aim ahead of the player's movement instead of chasing their current position
- Custom collision detection: line-circle intersection for projectile hits, circle-circle separation for enemy-enemy overlap

## Notes

This is an unfinished, quick passion project — built specifically to experiment with multiple enemy AI systems working together (orbiting vs. predictive-chase behavior) alongside custom collision detection, not as a polished or complete game. The player currently cannot take damage from enemy projectiles (`regPlayerHit()` is a stub), and there's no win/lose state yet.
