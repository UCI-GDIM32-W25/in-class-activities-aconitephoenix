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