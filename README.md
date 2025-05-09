# PaperZD 2.5D Template - Free for Use!

Developed with **Unreal Engine 5** using the **PaperZD Plugin**, this template provides a foundation for creating 2.5D platformer games with hack-n-slash combat. It blends classic platformer mechanics (think Mario) with an engaging attack system.

## Base Systems:

-   **Stats Component:**
    -   Easily manage health, defense, damage, and other attributes for various entities.
    -   **Damage Calculation:** Implements a dynamic damage system where damage dealt is influenced by the attacker's attack stat and the defender's defense stat.
        -   Formula: $\text{total damage} = \text{base damage} \times \frac{\text{attack}}{\text{attack} + \text{defense}}$
    -   Simplifies the creation of diverse enemies with unique combat characteristics.

-   **Dialogue Component:**
    -   Facilitates in-game conversations with NPCs and potentially bosses.
    -   **Datatable Driven:** Dialogue content is managed through easy-to-edit datatables.
    -   Utilizes a custom **struct** for streamlined data handling.

-   **Sprite Flicker Component:**
    -   Adds visual feedback upon taking damage or other events.
    -   Allows setting independent flicker durations for different object/enemy types.
    -   Features a configurable flicker timer (float).

## Attack System:

-   **Linetrace for Hit Detection:**
    -   Employs linetracing instead of complex collision shapes for attack registration.
    -   Optimized for 2D projects, offering good performance without the overhead of detailed collision management.

-   **Expandable Combo System:**
    -   Implemented within the Animation Blueprint (AnimBP) using sprite sheets.
    -   Built upon a tutorial framework with significant expansion and clear comments for easy modification.
    -   Utilizes a **tree-based system** for combo execution. For example, repeatedly pressing a light attack (L) can trigger a sequence like L, L, L, L, similar to many hack-n-slash games.

## Dialogue System:

-   **Customizable Choices:** Enables interactive dialogues with branching options for the player.
-   **Leaving NPCs:** Currently functions as if the conversation continues, but the ability to exit dialogue will be implemented in a future update (hopefully soon!).
-   **DataTable Driven Flow:** Simplifies dialogue management, allowing for easy drag-and-drop assignment of conversations to NPC Blueprint classes.

## Objects:

Contains a dedicated "Objects" folder with base classes designed for 2D elements using PaperZD. While standard Actor Blueprints could be used, these classes offer integrated functionalities like flipbook handling.

-   Includes a **Damage Interface** (`BPI_Damageable`) for consistent damage application and reception across different object types.

-   **Two Base Classes:**
    -   **3D (WIP):** Supports both Skeletal and Static Meshes, catering to various animation needs. Currently under development with a focus on expanding animation capabilities.
    -   **2D:** Utilizes Paper Flipbooks for visual representation. Implements basic damage handling and simple actor destruction upon overlap.

## Enemies:

Features two initial enemy types, with plans for future expansion and refinement.

-   **Turret:**
    -   Uses **Pawn Sensing** to detect the player.
    -   Spawns a bullet Blueprint object upon detection.
    -   Currently rotates on both vertical and horizontal axes (intended to be vertical-only; a fix is planned).

-   **Skeleton:**
    -   A basic enemy with health and damage attributes.
    -   Currently lacks AI behavior to actively attack the player but reacts to damage and can be defeated with a sprite flicker effect.
    -   **Future Enhancements:**
        -   Simple AI implementation, including edge detection.
        -   Functionality for the skeleton to see and attack the player.

## UI:

Includes three basic Widget Blueprints with preliminary code:

-   **Death/Respawn Screen**
-   **Main Menu**
-   **Main Player HUD**

## Instructions:

1.  Click the green "Code" button on the repository.
2.  Select "Download ZIP".
3.  Extract the downloaded ZIP file to your Unreal Projects folder or any other desired location.

*Side Note: This was my first experience with Git version control, so feedback on the repository structure is welcome!*

## Images:

![Gameplay Screenshot 1](https://github.com/user-attachments/assets/4aee32ab-6400-403e-b8c7-ea4c424974fe)
![Gameplay Screenshot 2](https://github.com/user-attachments/assets/a0eed4ed-6e23-41cb-9a3d-9870bef12766)

#### End/Credits:

I'm an enthusiastic hobbyist who learns through resources like YouTube, itch.io, and personal study. I enjoy creating templates to help others in the game development community. I hope this template proves useful for your projects, and I plan to release more updates and additions in the future. Feel free to use, modify, and build upon this foundation!

# Assets Used:
Main Player: https://clembod.itch.io/warrior-free-animation-set
Skeleton: https://jesse-m.itch.io/skeleton-pack
