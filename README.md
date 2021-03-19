# Pre-work - _Memory Game_

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program.

Submitted by: **Ryan Chang**

Time spent: **4** hours spent in total

Link to project: https://glitch.com/edit/#!/witty-celestial-tern

## Required Functionality

The following **required** functionality is complete:

- [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
- [x] "Start" button toggles between "Start" and "Stop" when clicked.
- [x] Game buttons each light up and play a sound when clicked.
- [x] Computer plays back sequence of clues including sound and visual cue for each button
- [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess.
- [x] User wins the game after guessing a complete pattern
- [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

- [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
- [x] Buttons use a pitch (frequency) other than the ones in the tutorial
- [x] More than 4 functional game buttons
- [ ] Playback speeds up on each turn
- [x] Computer picks a different pattern each time the game is played
- [ ] Player only loses after 3 mistakes (instead of on the first mistake)
- [ ] Game button appearance change goes beyond color (e.g. add an image)
- [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
- [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [x] Added 3 difficulty settings.

## Video Walkthrough

Here's a walkthrough of implemented user stories:

_Easy:_
![Easy](https://cdn.glitch.com/08075045-03e0-43f1-b864-22a31d82ea8b%2Feasygame.gif?v=1616140521968)

_Medium:_
![Medium](https://cdn.glitch.com/08075045-03e0-43f1-b864-22a31d82ea8b%2Fmediumgame.gif?v=1616140530500)

_Hard:_
![Hard](https://cdn.glitch.com/08075045-03e0-43f1-b864-22a31d82ea8b%2Fhardgame.gif?v=1616140528518)

_Fail:_
![Fail](https://cdn.glitch.com/08075045-03e0-43f1-b864-22a31d82ea8b%2Ffailgame.gif?v=1616140527184)

## Reflection Questions

1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here.

- https://www.w3schools.com/js/js_random.asp
- https://www.w3schools.com/jsref/jsref_push.asp
- https://www.seventhstring.com/resources/notefrequencies.html
- https://www.w3schools.com/cssref/css_colors.asp
- https://www.w3schools.com/js/js_arrays.asp

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words)

   I faced a few challenges when creating this submission:

   1. Randomly setting the pattern.

   - I was able to fix randomly setting the game pattern through using the Math.random() function. Coming from a C++ background, I had trouble with producing random whole numbers,
     instead of integers. Through some research, I discovered that Math.floor() will round down the current value at hand, which solved this issue.
     Furthermore, I had to research the syntax for JavaScript arrays.

   2. Creating different levels.

   - In order to create different levels, I had to modify the start game and stop game functions. Originally, we only had to worry about 1 start and 1 stop button.
     By following the pattern of creating buttons, and introducing parameters to the start game method, I was able to pass in different values based on the desired difficulty.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words)

   One question that I have about web development after completing this submission is: how do accounts work? More specifically, on many websites currently,
   there often exists a place for users to log in to an account. How could JavaScript be used to store the data of (in the case of large social media sites) millions of
   users, all with encrypted details? By completing this project, I have become aware of how much more I can learn about web development.

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words)
   If I had a few more hours to work on this project, I would spend them fixing two bugs and possibly one addition:

   1. Currently if the user holds down the mouse button, drags away from the button, then releases the mouse, the sound will not stop playing until another event is triggered.

   - I could complete this by possibly adding a class to the body which adds the functionality to pause the current sound that is being played.

   2. I would add a quality of life fix where inputs before the sequence of buttons has been played will not be counted toward the player's answer.

   - I could add a boolean variable which says sequenceNotComplete, and while the sequence is not complete, then ignore any button inputs.

   3. A feature I could add is a "infinite" mode, alongside a leaderboard.

   - Users could keep playing until they make a mistake, and then submit their high score to the leaderboard.
     I believe that this would take the longest to implement with my current abilites in JavaScript and HTML.

## License

    Copyright Ryan Chang

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
