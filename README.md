---

# 🔥 AAG: Dynamic Difficulty Flappy Bird Clone

A challenging take on the classic endless flyer, featuring dynamic difficulty scaling, a progressive visibility reduction effect, and satisfying sound design.

---

## 🎮 How to Play

### Controls

| Action | Key |
| :--- | :--- |
| **Start Game** | `ENTER` |
| **Jump** | `SPACE` |
| **Toggle Hitboxes** | `H` |
| **Restart** | `ENTER` (on Game Over) |

### Objective

Navigate the **Flaming Pipes** for as long as possible. The game gets progressively harder the longer you survive!

---

## ✨ Features & Dynamic Difficulty

The game environment and avatar change in response to your score, ramping up the challenge significantly:

* **Progressive Reduced Visibility (Vignette):** After reaching a score of **5**, a **darkening vignette effect** begins to appear, limiting your peripheral vision. This effect intensifies as your score increases.
* **Increasing Scroll Speed:** After reaching a score of **10**, the game begins to **speed up** gradually, forcing faster reactions.
* **Avatar Growth:** At a score of **10**, your avatar's size (and therefore its **hitbox**) increases by **50%**, making it much harder to fit through the pipe gaps.
* **Explosive Game Over:** When you hit a pipe or the ground, your avatar triggers an animated **explosion** accompanied by a dedicated sound effect.
* **Sound Feedback:** Satisfying sound effects (SFX) are included for jumping, scoring points (every 5 points), and triggering the game over state.

---

## 💻 Setup and Running Locally

Since this game is built using pure HTML, CSS, and JavaScript, it is extremely easy to run.

### Requirements

To run this project with all features intact (especially sounds and images), you **must** have all the asset files in the same directory as the `index.html` file.

| Assets (Images) | Assets (Sounds) |
| :--- | :--- |
| `bg.png` | `jump.mp3` |
| `p.png` | `score.mp3` |
| `pi.png` | `gameover.mp3` |
| `av.png` | `explosion.mp3` |
| `f1_s_70.png` | |
| `f2_s_70.png` | |
| `f3_s_70.png` | |
| `explosion.png` | |

### Steps

1.  Save the provided HTML code as `index.html`.
2.  Gather all 11 required image and sound files.
3.  Place all files (`index.html` and the 10 assets) into a single folder.
4.  **Double-click `index.html`** in your file explorer. It will open automatically in your default web browser and be ready to play!

---

## 🔧 Customization

The game is heavily configurable using the `CONFIG` object in the `<script>` tag. Key variables you might want to adjust include:

| Variable | Description |
| :--- | :--- |
| `CONFIG.gravity` | Controls how fast the player falls. |
| `CONFIG.jumpForce` | Controls how high the player jumps. |
| `CONFIG.pipeGap` | The vertical distance between the top and bottom pipes. |
| `CONFIG.avatarGrowthScore` | Change the score needed for the avatar to grow. |
| `CONFIG.avatarGrowthScale` | Change the scale factor of the growing avatar (e.g., 2.0 for double size). |
| `CONFIG.vignetteStartScore` | Change the score when the darkening effect starts. |
