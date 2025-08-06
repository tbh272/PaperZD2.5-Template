# 🕹️ PaperZD 2.5D Template - Free for Use!

🎮 Build your own 2.5D hack-n-slash platformer with a solid starting point!  
Made with **Unreal Engine 5** and the **PaperZD Plugin**, this template combines classic platforming like *Mario* with light hack-n-slash combat systems.

---

## 🆕 Update 1.3 Highlights

🗺️ **Demo Map Added**  
Explore a new demo map that shows off all current features and systems.

📦 **Combined Content**  
All previous updates are now merged into 1.3.  

---

## 📥 How to Get Started

1. Download the latest release on the right hand side.
2. Select **"Download ZIP"**.
3. Unzip it to your **Unreal Projects** folder (or wherever you prefer).
4. Open the project in **Unreal Engine 5**, and you're good to go!

---

## ⚙️ Base Systems

### 🧠 Stats Component

- Manage stats like health, defense, and attack.
- 💥 **Damage Formula**:  
  `total damage = base damage × (attack / (attack + defense))`
- Makes it easy to create enemies with different strengths.

### 💬 Dialogue Component

- Basic conversations with NPCs (and possibly bosses later).
- Driven by **DataTables** — easy to update!
- Built with a clean custom **struct** for managing text.

### ✨ Sprite Flicker Component

- Gives feedback when characters or objects take damage.
- Flicker time can be customized for each object/enemy.
- Built using a simple float-based timer.

---

## 🗡️ Attack System

### 🎯 Hit Detection with Line Traces

- Uses line traces instead of collision boxes for hits.
- Clean and fast for 2D gameplay.
- You can add attacks without adjusting every frame of the animation.

### 🧩 Expandable Combo System

- Tree-based combo attacks, like: `L > L > L > L`
- Easy to extend using the **Animation Blueprint (AnimBP)**.
- Built on a tutorial base, but heavily expanded with comments to help you understand and change it.

---

## 💬 Dialogue System (More Details)

- Supports **choices** in conversations.
- Leaving NPCs mid-dialogue isn’t implemented yet — but it’s planned!
- Works by dragging and dropping conversations using DataTables into NPC Blueprints.

---

## 🧱 Objects Folder

A special folder for base objects that work with **PaperZD**.

- Includes a **Damage Interface** (`BPI_Damageable`) so anything can take damage consistently.
- **2D Base Class**:
  - Uses Flipbooks.
  - Handles damage and self-destruction on overlap.
- **3D Base Class (WIP)**:
  - Supports Skeletal and Static Meshes.
  - Still in development to expand animation features.

---

## 👾 Enemies

Two example enemy types included, with more to come:

### 🧍‍♂️ Skeleton

- Has health and reacts to damage.
- Doesn’t attack yet, but dies with a flicker.
- 🧠 Planned Improvements:
  - Basic AI (walk, detect edges, chase player)

### 🧨 Turret

- Uses **Pawn Sensing** to detect players.
- Spawns bullets when it sees you.
- Rotates on X and Y (will be limited to vertical-only soon).

---

## 🧾 UI System

Includes 3 basic **Widget Blueprints**:

- 🪦 Death / Respawn Screen
- 🏠 Main Menu
- 🎯 Player HUD

Simple layouts that can be replaced with your own designs!

---

## 📸 Screenshots

### Demo Gameplay  
![Gameplay Screenshot 1](https://github.com/user-attachments/assets/4aee32ab-6400-403e-b8c7-ea4c424974fe)

### Combat and UI  
![Gameplay Screenshot 2](https://github.com/user-attachments/assets/a0eed4ed-6e23-41cb-9a3d-9870bef12766)

---

## 🔜 Coming Soon

- Skeleton AI that can chase and attack
- More polish to dialogue (like exit options)
- Additional example enemies and test maps
- Visual effects and audio for combat hits

---

## 🎨 Assets Used

- [Main Player](https://clembod.itch.io/warrior-free-animation-set)
- [Skeleton](https://jesse-m.itch.io/skeleton-pack)
- [Low Poly Assets](https://craigsnedeker.itch.io/classic64-asset-library)

---

## 🙌 Final Notes

While I am familiar with UE5, I am learning through YouTube, itch.io, and trial and error.  
This was my first time using Git version control — if the repo structure seems messy, feel free to send feedback!

💡 This template is totally free — use it, break it, build on it, make it your own!  
If you make something cool with it, I’d love to see it.  
Thanks for checking it out!

