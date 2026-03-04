# GDIM32 In Class Activities
## W1
### Activity 1
Predict how much time you'll take on a minigame before you procrastinate (or just don't procrastinate in general!!)
### Activity 2
1. 10
2. 2
3. Prints "hello world" to the console every frame
4. MonoBehaviour
5. Prints "x = 10" to the console when the game starts
6. Method argument + parameter, argument passes value thru parameter to run method
7. Translate can only be called on an object, not a class (Transform)
8. Change it to _playerTransform
### Activity 3
[Link to doc](https://docs.google.com/document/d/1ZloeI2O3HLCZUm7UvvfKdylog4EuKHg3eZPcW1Tevz0/edit?usp=sharing)
## W2
### Activity 1
![Xvwz0k4l](https://github.com/user-attachments/assets/78cc67f9-b668-48eb-b2b2-089694fa0fde)
### Activity 2
[Mainly collider code and figuring out movements (player jump, coin moving, etc.)](https://github.com/UCI-GDIM32-W25/mg2-aconitephoenix/commit/79e1a2643450d0d9ef5eeda8539196e1645c7b02)
## W3
### Activities 0-2
Buddy name: Eli
### Activity 3
<img width="1810" height="1513" alt="Screenshot 2026-01-20 174637" src="https://github.com/user-attachments/assets/1630a79a-38f6-4a6a-9d4f-e7ecbca9e783" /> 

## W4
### Activity 0
Buddy name: Eli
### Activity 1
At runtime (`Awake()`), the `Locator` script logic checks for extra instances of a `Locator` object and destroys them. This prevents multiple instances of a `Locator` object from existing, making sure it's a singleton.
### Activity 2
![IMG_0426](https://github.com/user-attachments/assets/05c0c74d-051b-4ac2-bed4-e861d22656a2)
![IMG_0425](https://github.com/user-attachments/assets/aa603ce3-3b1c-49f7-8873-134e668f2c17)
### Activity 3
[I added the bird and pipe sprites and spliced them properly. I also added the ground and bird object to the scene. Unfortunately could not get any farther because my computer was nearly about to die and I didn't bring a charger...](https://github.com/aconitephoenix/HW4/commit/f601fb74d717b28fa7b38bd4104fb085a36bc9e1)
## W5
### Activity 1
I feel like I would change IBreakable from an interface to an abstract, mainly because it seems that the IBreakables have a durability that cannot be implemented in the parent class because interfaces cannot have member variables. I feel like Item and IBreakable could switch abstract and interface. In general, I do feel like the game data should be stored in something like a ScriptableObject as well.
### Activity 2
The EnemyStats and ItemW5Demo2 classes are the Models as they contain game data. The DialogueBubble and InventoryUI classes are the Views as they mainly work on displaying visual information in the game. The Controllers are the EnemyW5Demo2 and PlayerW5Demo2 classes as they handle the game logic.
### Activity 3
#### Scenario 1
- beats represented by prefabs to be able to map multiple of them across the screen
- scriptableobjects contain data about the beats in the song + the types of beats they are
#### Scenario 2
- stats for abilities = model, gameplay code performing abilities (causing dmg, creating shields) = controller, ui for abilities + results = view
#### Scenario 3
- finite state machine for player animations (different states activate different animations)
- inheritance w polymorphism for the different plants/rocks
    - probably abstract classes so that the parent class can have empty methods that plants can implement with their own bodies, but also so they'll have inheritable member variables and stuff
- scriptableobjects used to store inventory data + plant properties
- model stores the properties of the plants and such, view renders the animations/ui, controller controls game logic (player actions)
- singleton locator to allow all classes to access player's events
### Activity 4
Attendance: Sebastian Magana, Kaleb Reyes, Jess Tran  
Proposal: [Final Project Proposal First Draft](https://docs.google.com/document/d/11WOaLqc5etO8rKHDXbb_FdNeKd7ZzC0tJGFpK8PWQyE/edit?usp=sharing)
## W6
### Activity 1
#### Gizmos
- gizmos allow you to see the distance btwn 2 objects before they collide w each other to check collider sizes
- helps to diagnose issues a lot faster via visualization
- remember: gizmos are only visible in SCENE VIEW!!!!!
- in demo, velocity collider shows the velocity + direction of the object as it moves
- circle collider shows direction capybara is facing
#### Profiling
- Profiler allows to see performance details
- helps to figure out what methods are taking longer to execute
- for the specific demo, the fruit had a weird polygon collider that had a bunch of unnecessary joints
- not a good idea to have multiple objects with really detailed colliders in the same scene
- circle collider is most efficient collider for the fruit
- after changing fruit prefab, method runtimes bc more even
- learning abt optimization and performance is important!!! good skill for your resume
- CPU runs all program logic
- GPU renders all the frames
#### Breakpoints
- makes diagnosing errors easy bc the code stops running the moment it hits the breakpoint
- unity application becomes completely paused at breakpoint
- in demo, discovered that instance was null
- you get to see the chain of events that led up to the breakpoint!
- in demo, replace start w awake
- don't have to write debug lines w breakpoints!
### Activity 2
Attendance: Jess Tran, Kaleb Reyes (Sebastian went to GDW!)  
Proposal: [Final Project Proposal Final Draft](https://docs.google.com/document/d/11WOaLqc5etO8rKHDXbb_FdNeKd7ZzC0tJGFpK8PWQyE/edit?usp=sharing)
## W7
### Activity 1
- gizmo on duck represents how far he can see
- once duck can see you he starts pursuing you
    - can be blocked by obstacles (tree)
- duck has FSM to change behavior/movement based on what's in its line of sight
    - makes things more organized
- raycasting useful for coding aggro-ed enemies
    - makes sure they don't attack you too fast/early
### Activity 2
Attendance: Jess Tran, Sebastian Magana, Kaleb Reyes
### Activity 3
<img width="1300" height="1284" alt="Final Project Breakdown" src="https://github.com/user-attachments/assets/d3dd5ada-1889-40bd-a120-d5b401eb77ff" />

### Activity 4
[Link to Trello Board](https://trello.com/invite/b/69951f944f330958a4e6bf2f/ATTI692e766e2b54a385c7f1c25f3ba63f9b039DA622/goofy-goobers-final-tasks)
### Activity 5
[I imported the TMP Text assets into the game and added a basic UI element to represent the pages collected.](https://github.com/lindenreid/GDIM32-Final/commit/3e0f7756599589383785c1ce3db733847201f71d)
## W8
### Activity 1
- post-processing - shaders that affect the look of your entire screen
    - ex: bloom (makes things glow and stuffff)
- can change the tint of the camera to give things a cohesive look
- wiggle effect in witcher III is a post-processing effect, can identify bc its affecting the entire screen
- unity packages are fine to use for final project!!!
- you hit "add effect" on the post processing thing and you can just add the effect
    - usually they come with their settings off by default for some reason so make sure you turn that on
### Activity 2
Attendance: Jess Tran, Sebastian Magana, Kaleb Reyes
### Activity 3
- Player movement is good and responsive
- Sprint bar and sprint depletion works
- Jumped off world, need to add terrain and boundaries
- Itch description for controls is good, need to add click to interact when implemented
### Activity 4
Task: Working on dialogue triggers
### Activity 5
[I worked on the dialogue trigger activating when the player clicked on an NPC (it only semi-works right now...)](https://github.com/aconitephoenix/GDIM32-Final/commit/091bb4997f8086299890249265e2237477873253) 
## W9
### Activity 1
- diff number of options per branch
- the stray kids and shinee options only lead to one option, BTS leads to more options
- multiple dialogue branches makes it easy for designers to edit the lines
- there are also nodes to return to, kind of like a foldback structure
- for multiple NPCs with branching dialogue options
    - canvas code should hook the button up to the NPC that's actually talking
    - have some function that, when you press the button to interact w the npc, to assign the inputs to the correct NPC + keep note of what dialogue node is currently active
    - code should be separate from the NPC
    - move dialogue logic to dialoguecontroller, NPC stores other info
### Activity 2
Attendance: Jess Tran, Sebastian Magana, Kaleb Reyes
### Activity 3
- He liked how it gave clear instructions to get the page
- Need to add indicator or highlight on the page so that its more clear where to go
- Indicator for the NPC that they are interactable
- Add the rest of the content
- Add Compass for page navigation (Slenderman Tentacle)
### Activity 4
As of now, we're pretty much halfway through our project and on pace!! We just need to further polish the content and logic of the game.
### Activity 5
[I fixed an issue with the dialogue where if you clicked off the buttons while the player options were active, the dialogue would close. That no longer happens now!!! Hopefully!!!!!](https://github.com/aconitephoenix/GDIM32-Final/commit/087bba7aa81ce077f3caa8391548918f52119a58)