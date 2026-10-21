
# spot-demo-public ₊˚⊹♡

**voice-controlled robotics · computer vision · autonomous movement**

a little side project where i taught Boston Dynamics Spot some new tricks! ♡

i originally worked with Spot during my summer 2026 research on voice-controlled navigation, but wanted to see what else i could teach him. now he can dance, do pushups, look pretty, and even move toward people when asked.

this is a public showcase of my project! the actual implementation lives in a private repository to protect robot-specific configurations and research information.

---

## about the project ✧

this project uses Python and the Boston Dynamics Spot SDK to turn spoken commands into robot movements.

i built the demo around offline speech recognition using Vosk, so Spot can understand commands without depending on an internet connection.

since he doesn't have an arm, all his tricks use body positioning, walking, and movement sequences. for some commands, he can also use LiDAR, depth sensing, and AprilTags to interact with his surroundings.

### tech stack ⋆｡°

`Python` · `Spot SDK` · `Vosk` · `Raspberry Pi` · `LiDAR` · `AprilTags` · `Computer Vision`

---

## meet spot's tricks ♡

| what you say | what spot does |
|---|---|
| "spot, say hi" | bows to say hello |
| "spot, look pretty" | stands tall and tilts his head |
| "spot, do a pushup" | does 3 pushups |
| "spot, pushup competition" | does 10 pushups and flexes |
| "spot, dance" | sways and bobs |
| "spot, nod" | nods yes |
| "spot, shake your head" | shakes his head no |
| "spot, spin" | checks for obstacles and spins |
| "spot, play dead" | rolls onto his side and gets back up |
| "spot, walk in a circle" | walks in a circle while checking his surroundings |
| "spot, go to them" | moves toward a detected person or visual marker |
| "spot, come back to me" | returns toward his remembered starting position |
| "spot, demo" | performs a little sequence of tricks ♡ |

---

## how it works ⊹

**01. voice input 🎤**

a microphone connected to a Raspberry Pi captures spoken commands.

**02. speech recognition**

Vosk processes speech locally and converts it into text.

**03. command matching**

Python cleans the recognized text and matches it to one of Spot's supported tricks.

**04. environment checks**

movements that involve navigation use available LiDAR, depth sensing, or AprilTags to help identify locations and check surroundings.

**05. robot control**

the Spot SDK sends the corresponding commands to execute the movement.

### the pipeline ⋆｡°

```text
voice input
    ↓
offline speech recognition (Vosk)
    ↓
text processing + command matching
    ↓
environment + safety checks
    ↓
Boston Dynamics Spot SDK
    ↓
robot movement ♡
```

---

## demo time! ˚₊‧꒰ა ♡ ໒꒱‧₊˚

*coming soon...*

i'm planning to add videos of Spot performing his tricks here!

---

## behind the project ✿

this started as a fun extension of my summer 2026 research, where i developed a voice-controlled navigation system for Boston Dynamics Spot.

i wanted to move beyond telling Spot where to go and experiment with how he could interact with people through movement and speech.

one of my favorite challenges was figuring out how to make a robot without an arm perform recognizable gestures. it took a lot of experimenting with body positioning, timing, and different movement sequences.

this project gave me more experience with robot control, speech recognition, sensor integration, and building software that actually interacts with the physical world.

---

## related research ୨୧

**voice command navigation for Boston Dynamics Spot — summer 2026**

my earlier research focused on connecting speech recognition with Spot's GraphNav system to navigate between mapped locations using natural language commands.

this trick demo builds on that work by focusing on interactive behaviors and movement instead of waypoint navigation.

---

## a little note ♡

the source code is kept private because it includes robot-specific configurations and research-related information. this repository is meant to showcase the project's design, technical features, and demonstrations.

---

made with ♡ by [lexi tinajero](https://github.com/lexitinajero)

˚₊‧꒰ა ♡ ໒꒱‧₊˚
