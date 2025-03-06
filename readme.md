# Chomper

**Chomper** is a fun, web-based augmented reality (AR) game that uses your webcam and face tracking to let you “chomp” edible objects while avoiding poisonous ones. The game utilizes Mediapipe FaceMesh for real-time face tracking and A-Frame for 3D rendering and AR environment. 

## Features

- **Real-Time Face Tracking:**  
  Uses Mediapipe FaceMesh to track your face and position a cursor based on your face center. The video feed is mirrored so that your movements feel natural.

- **Dynamic Gameplay:**  
  Randomly spawned shapes (edible objects in green and poison objects in red) move toward you. Open your mouth when the edible object aligns with your face to “eat” it and score points.


- **User Interface:**  
  - **Start Modal:** On page load, a modal explains the game ("Chomper") and its instructions.
  - **Game Info Display:** Shows the current score and health (alive/dead) at the top-right.
  - **Credits Button:** Located below the score card. Clicking it reveals a modal with detailed credits and asset licenses.
  - **Game Over Modal:** When you eat a poison object, a modal displays your final score and offers a restart button.

- **Privacy-Focused:**  
  The camera is only activated while the game is in play and is turned off when the game ends.


## How to Play

1. **Start the Game:**  
   When the page loads, you’ll see the start modal with the title **Chomper** and instructions. Click **Play** to begin.

2. **Gameplay:**  
   - Align your face with incoming objects.  
   - Open your mouth to “eat” edible objects (green) and avoid poison objects (red).  
   - Each edible object you eat increases your score.

3. **Game Over:**  
   If you “eat” a poison object, the game ends, and a game over modal appears displaying your final score along with an option to restart.

4. **View Credits:**  
   Click the **Credits** button (located below the score card) to view detailed credits and asset licenses in an overlay. Click outside the credits modal or the close button to dismiss it.

## Requirements

- A modern web browser that supports **getUserMedia** and **WebXR** (e.g., Chrome, Firefox).
- The game must be served over HTTPS to access your webcam.
- No additional installation is required; simply open the HTML file.

## Getting Started

1. **Clone or Download the Repository:**  
   Clone this repository or download the source files.

2. **Configure Assets:**  
   Update the asset paths in the HTML file for:
   - Background music (`bg-music-sound`)
   - Collision sound (`collision-sound`)
   - Any custom 3D models (e.g., cake)

3. **Serve Over HTTPS:**  
   Use a local server or hosting environment that serves files over HTTPS. For example, you can use a tool like [http-server](https://www.npmjs.com/package/http-server) with SSL enabled.

4. **Open the Game:**  
   Open `index.html` in your supported web browser to start playing.

## Code Overview

- **index.html:**  
  Contains the complete game code:
  - A-Frame scene setup and environment components.
  - Mediapipe FaceMesh integration for face tracking.
  - Game logic for object spawning, collision detection, scoring, sound, and particle effects.
  - HTML modals for game start, game over, and credits.

## Credits

The game uses various assets; here are some of the credits (full details are shown in the Credits modal):

- "Handpainted watercolor cake" ([link](https://skfb.ly/oH9yt)) by Anna Espenstein – Creative Commons Attribution.
- "Mouthwatering banana pancakes in syrup" ([link](https://skfb.ly/oW9Gy)) by nottodayrender – Creative Commons Attribution.
- "Potion bottle (poison)" ([link](https://skfb.ly/onYxP)) by Ret.ouchs – Creative Commons Attribution.
- "POISON GLASS BOTTLE" ([link](https://skfb.ly/6WMQq)) by Studio Sazor – Creative Commons Attribution.
- "Extra Chocolate Marshmallow Cupcake" ([link](https://skfb.ly/onoCB)) by jtressle – Creative Commons Attribution.
- "Lasagna" ([link](https://skfb.ly/oXoRA)) by UmangRank – Creative Commons Attribution.
- Nom Noise by TheDragonsSpark – [link](https://freesound.org/s/543386/) – License: Attribution 4.0.
- Eating a cracker (Mouth open) by Rudmer_Rotteveel – [link](https://freesound.org/s/364923/) – License: Creative Commons 0.
- crunch 4.wav by theplax – [link](https://freesound.org/s/608639/) – License: Attribution 4.0.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions, bug reports, and feature requests are welcome! Feel free to fork the repository and submit pull requests.

## Acknowledgments

- [A-Frame](https://aframe.io/) – for the amazing WebVR/AR framework.
- [Mediapipe](https://mediapipe.dev/) – for real-time face tracking capabilities.
- All asset creators whose work is credited in the game.

---

Enjoy playing **Chomper** and happy chomping!

