# Pre-work - *"Remember Me?" Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Christian Bryan**

Time spent: **16** hours spent in total

Link to project: https://glitch.com/edit/#!/certain-guiltless-passbook

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [x] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [x] Player only loses after 3 mistakes (instead of on the first mistake)
* [x] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:
* [x] Confetti shower once the player wins the game!

## Video Walkthrough (GIF)

Start, Stop, Pattern functionality:
![Start](https://user-images.githubusercontent.com/77913247/164305948-b00b021b-4545-4793-8a22-2a583543e07d.gif)

Mistake Counter:
![mistake](https://user-images.githubusercontent.com/77913247/164305987-8259770f-759a-4d06-af1c-fd6d721ec4c3.gif)

Winning Game:
![win](https://user-images.githubusercontent.com/77913247/164306019-89f30cfa-fbe0-4807-8970-e12c13301390.gif)

Losing Game:
![lose](https://user-images.githubusercontent.com/77913247/164306041-8d144e60-3da2-4f5f-8b57-1d76fd3de0c2.gif)

GIFs created with [LiceCap](https://www.cockos.com/licecap/)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
* Confetti Shower source code [CSSscript](https://www.cssscript.com/confetti-falling-animation/)
* Confetti Shower Troubleshooting [YouTube](https://youtu.be/D8D9AvsowbY)
* JavaScript reference for randomizing numbers (used for random pattern): [StackOverflow](https://stackoverflow.com/questions/4959975/generate-random-number-between-two-numbers-in-javascript)
* Cute Animal Photos: 
  * Bunny: [Unsplash.com](https://unsplash.com/photos/S0aPskfdJGY)
  * Puppy: [Unsplash.com](https://unsplash.com/photos/z_U6bPp_Rjg)
  * Cow: [Unsplash.com](https://unsplash.com/photos/VW-Cu5FJjSM)
  * Sheep: [Unsplash.com](https://unsplash.com/photos/1j9Yrl0nW10) 
  * Duck: [Unsplash.com](https://unsplash.com/photos/J0UeiNjSkxc)
  * Fish: [Unsplash.com](https://unsplash.com/photos/VyFdgN2UYeU)

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

Duck…sheep…chicken… “Congratulations, you remembered!” I attentively play my memory game for likely the hundredth time when that familiar message appears. Although I have won the game, my success is underwhelming. My game resets back to its original state, no celebration, no prize, just a start button that reappears longing for me to play again. I thought for a moment, as much as the cute puppy, cow, and other baby animals that hid beneath the buttons intrigued me, I wished for something more…something unexpected, then it hit me – a confetti cannon. 

Having no previous knowledge of Javascript, I soured google for a confetti cannon implementation that I could utilize in my project, I found a simple source (mentioned above) that seemed like it could be realistically implemented. Thus, I began the process of trial and error. After exploring the confetti source code I found the startconfetti() and stopconfetti() functions that I could implement in my wingame() and startgame() functions and *BAM* there it was, confetti…but not in the right spot. The confetti only appeared below my buttons, not quite the full webpage shower I was looking for. I tried a multitude of things, making the confetti into a paragraph element, creating a div with a paragraph element that utilized the document.getElementById() feature in my own Javascript, and making a canvas element that I attempted to alter the style of in my CSS file. Unfortunately, none of those options were successful, my confetti was still trapped below my buttons and I was getting concerned that it would be trapped there forever. However, my time in computer science has taught me that there is always a way, thus I moved away from HTML, JS, and CSS reference sites and into the realm of YouTube tutorials. My journey of trial and error continued and my files took many forms until I noticed an individual alter the CSS of a canvas in their JS file that allowed their confetti to cover the entire webpage. I search the confetti source code and found a canvas embedded in the script, I then altered the CSS styling of the canvas, and suddenly my 4 hours of confetti cannon “debugging” became all worth it as I watched confetti pour down my webpage upon winning the game. 

Though my understanding of HTML, JS, and CSS was limited, I was able to iterate through the challenge and find the unexpected, colorful surprise I was looking for. 


3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

Although I was able to get my project working successfully and with the features I wanted to add, I felt that certain challenges I encountered along the way could have been more efficiently solved if I knew how to debug in JS, HTML, and CSS. On an HTML reference site, I noticed that the terminal, accessed by the inspect element, was used to track the value of specific variables mentioned in the Javascript. I would love to learn how to use the terminal when conducting web development as it allows me to visualize the way my code runs, giving me a greater understanding of my computer’s interpretation of the code. With the skill of debugging, I feel that I could obtain a better foundation of web development, enhancing my programming skillset. 

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

In school thus far, I have only had the opportunity to work on backend projects. I truly enjoyed working on the memory game as it afforded me a visual and auditory creativity that I have not experienced before in the programming realm. If I had the opportunity to continue with this project, I would implement the timer, and altered game button sounds, likely sounds that align with the animal photos I placed under the buttons. Another sound feature I would like to add is low-volume elevator-style background music. From my experience playing simple online games, background music that can be toggled by the user has always made the game more inviting and I believe it would do the same for my game. Lastly, with my newly learned knowledge of confetti cannon implementation, I would like to apply a different particle pop-up when the user loses the game, such as sad faces which I feel will make the game more interactive with the player. 



## Interview Recording URL Link

[My 5-minute Interview Recording](your-link-here)


## License

    Copyright Christian Bryan

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
