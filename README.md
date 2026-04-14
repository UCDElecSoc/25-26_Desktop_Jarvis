# Desktop Robot Assistant  
### A Raspberry Pi–powered embodied AI assistant with voice, vision, expressive display, and real-world hardware control

<p align="center">
  <em>An interactive desktop robot that can listen, speak, see, think, display expressions, and act through hardware.</em>
</p>

---

## Overview

This project is a **smart desktop robot assistant** built around a **Raspberry Pi 5**, designed to bring AI out of the screen and into the physical world.

Instead of functioning as just another chatbot or speaker assistant, this robot is intended to become a more embodied system: one that can **hear spoken commands, reason through an LLM, observe the environment through a camera, display expressive facial animations on an external screen, and execute actions through hardware and software control**.

At its core, the project explores the intersection of:

- **embedded systems**
- **robotics**
- **voice interaction**
- **computer vision**
- **agent-based AI**
- **human-robot interaction**

This repository currently serves as a **project showcase and technical overview**. The source code is not public at this stage.

---

## Project Vision

The goal is to build a robot that feels more alive, more interactive, and more useful than a standard voice assistant.

The long-term vision is a robot that can:

- understand spoken requests naturally
- respond with voice and visual expressions
- observe its surroundings through a camera
- control hardware connected to the Raspberry Pi
- run useful actions on the local system
- eventually perform more autonomous and context-aware behaviours

In other words, this project is about creating a **physical AI presence on a desk**, not just another software interface.

---

## Key Capabilities

### Voice Interaction
The robot is designed to support a full speech pipeline:
- microphone input
- speech-to-text
- LLM-based reasoning
- text-to-speech output

This allows the system to hold natural spoken conversations while also using language as the command layer for physical actions.

### Expressive Face Display
A custom digital face is rendered on an external display connected to the Raspberry Pi.  
The current concept uses stylised animated eyes to create a cleaner and more robotic visual identity.

Planned expression features include:
- blinking
- glow effects
- eye movement
- emotion-inspired expression changes
- state-dependent visual feedback

### Visual Awareness
Using a raspberry pi camera module, the robot is intended to gain basic environmental awareness.  
This opens the door to features such as:
- object observation
- target tracking
- facial recognition
- vision-guided behaviours

### Hardware and System Control
A major part of the project is enabling the robot to interact with the real world through the Raspberry Pi itself.

This includes:
- executing shell commands
- opening local or web applications
- interacting with GPIO
- motor control
- distance and self-oriantation sensing

### Agent-Based Orchestration
The system uses **OpenClaw** as the orchestration and control layer between language intelligence and device-level execution.

This makes it possible for the LLM to go beyond conversation and become a controller for actual tools and behaviours.

---

## Why This Project Matters

Most AI assistants today remain confined to a screen, a browser tab, or a speaker.  
This project asks a more interesting question:

> What happens when an AI assistant has a body, a face, a voice, and access to hardware?

By combining LLM reasoning with embedded hardware, this robot becomes a platform for exploring:
- embodied AI
- human-machine interaction
- robotics prototyping
- multimodal interfaces
- physical AI products

It is both a technical challenge and a design experiment.

---

## System Concept

The interaction loop is designed around a full perception–reasoning–action pipeline:

User Speech
   ↓
[Local]
Microphone / Audio Input
   ↓
 [API]
Speech-to-Text
   ↓
LLM Reasoning
   ↓
[Local]
OpenClaw Agent Layer
   ├── Shell commands
   ├── GPIO / hardware control
   ├── Camera access
   ├── Screen / face control
   └── System feedback
   ↓
[Local]
Robot Response
   ├── Spoken reply
   ├── Visual expression
   └── Physical or software action
