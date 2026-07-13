# AI Robotics Projects — Research & Concept Selection

**Status:** Still researching — figuring out which of these two to actually build
**Working with:** an industry mentor (System Architect, Google)

## What this is

I'm exploring two robotics project ideas and trying to decide which one to build.
Both would use an AI model to actually make decisions (analyzing camera/sensor
input and choosing what to do) instead of just running pre-programmed behaviors.
This repo is where I'm keeping notes, part lists, and cost breakdowns as I
research each option.

## Idea 1: AI Companion Robot

A small robot that can drive around a room, avoid bumping into things or driving
off edges, and talk with you using an AI model for the "brain."

**What I've figured out so far:**
- Split the computing into two parts: a Raspberry Pi handles the camera/voice/AI
  side, and a separate ESP32 microcontroller handles driving and obstacle
  avoidance directly — that way the robot doesn't wait on an AI response just to
  avoid running into a wall
- Went with a simple 2-wheel drive + caster ball wheel setup instead of tank treads — easier to
  build and control at this size
- Planning to use camera attached to a full-rotation gimbal for visuals + edge/fall detection


## Idea 2: AI Drawing Robot

A desk robot that draws pictures — similar to the drawing-robot toys you can
find online, but instead of only drawing from a fixed set of preset images, it
would use AI to figure out how to draw whatever image you give it.

**What I've figured out so far:**
- The arm mechanism is two motors that each move an arm, and the two arms meet
  at a single pen holder (this is how a lot of the commercial versions work).
- Still looking into the arm mechanism and considering the possibility of two
  separate robot arms.
- Still researching how to control how hard the pen presses on the paper — the
  leading idea right now is a small force sensor (load cell) in the pen holder
  that can tell how much pressure is being applied, so the robot can keep it
  consistent instead of pressing too hard or too soft. Haven't built or tested
  this part yet.

## How I'm deciding between them

| What I'm weighing | Notes |
|---|---|
| How hard is it to actually build | |
| Rough cost | |
| How much new stuff I'd have to learn | |
| How long until I have something working | |

*(Still filling this out before picking a direction.)*

## Next steps

- [ ] Finish comparing the two ideas and pick one
- [ ] Model the components and assemble a basic structure
- [ ] Order the core parts and start prototyping
- [ ] Test the sensor/control logic on its own before building the full robot
