
**Labyrinth of Oblivion**
is a first-person 3D survival horror game developed in Unity. The player is trapped inside a dark, procedurally structured maze with a single objective: escape. To do so, the player must explore the environment, 
collect key items hidden in interactive chests, and evade a hostile AI-driven enemy that navigates the environment using real-time pathfinding.

**Game Description**
The gameplay is designed around strategic exploration and psychological tension. Players must find a lantern and a gun hidden within the maze to aid survival.
A key item required to unlock the exit door is randomly placed in one of the chests. Meanwhile, the player is hunted by an enemy using NavMesh-based pathfinding and a Finite State Machine (FSM) to switch between patrol, chase, and attack states based on player actions.

**Core Features**
-AI Behavior: Enemy controlled using a state-based AI system (Idle, Patrol, Chase, Attack), integrated with Unity’s NavMeshAgent for intelligent navigation.

-Chest-Based Inventory: Items like the lantern, gun, and key are stored in chests and can be collected through raycast-based interaction.

-AI Enemy: detects the player using spatial sound triggers (e.g., footsteps, interactions, dropped objects).

-Dynamic Lighting System: Lantern-based lighting and ambient effects simulate tension; lights can flicker or deactivate based on in-game events.

-Weapon System: A basic one-shot firearm mechanic is implemented with reload and limited use, triggered upon item pickup.

-Scene Management: Transitions between main menu, gameplay, death, and escape scenes are handled through Unity’s SceneManager.

**Technologies Used**
-Unity Engine (2022.3.x LTS) – Primary game engine

-C# – Scripting for gameplay mechanics, AI logic, and UI

-Blender – 3D modeling and animation (maze, props, character)

-NavMesh & FSM – Used for AI pathfinding and behavior transitions

-Unity Animator and Timeline – Used for event sequences and cutscene-style transitions


**Gameplay Flow:**
Player starts in a locked maze environment.

Chests scattered around the map can be opened to find the lantern, gun, and exit key.

The enemy continuously patrols or responds dynamically based on player-generated sound or visibility.

Upon acquiring the key, the player must return to the exit point and unlock the door to escape.

If caught, the player transitions to a death scene. Successful escape leads to the escape scene.

**Setup and Requirements:**
-Unity 2022.3 LTS or above

-Visual Studio with C# environment enabled

-Blender (for asset editing, optional)

-Minimum hardware: GPU with support for real-time rendering and shader processing

**Status:**
-Current Version: Prototype (Playable)

-Fully integrated gameplay loop with AI, item collection, and multiple outcomes

-Clean modular C# scripting for scalable feature addition

**Planned Enhancements:**

-Procedural maze generation

-Enhanced enemy variety and learning behavior

-In-game UI for health and inventory systems


