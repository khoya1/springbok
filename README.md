# Springbok Drawing Tool

A Java Swing application that renders an interactive, animated Springbok (a South African antelope). Built using object-oriented design principles including the **Decorator pattern**.

## Features

- 🦌 Draws a Springbok with body, head, legs, horns, eyes, mouth, neck, and tail
- 🎩 Toggle a hat on the Springbok
- 👟 Toggle shoes on the Springbok
- 🎵 Start/stop singing — plays audio and displays musical notes
- 🌿 Toggle a green background
- 📏 Resize the Springbok using a slider

## Project Structure

```
src/drawingTool/
├── DrawingTool.java         # Main JFrame with control panel (entry point)
├── DrawingArea.java         # Canvas panel
├── Scene.java               # Manages drawing state
├── Springbok.java           # Core Springbok model
├── Animal.java              # Animal interface
├── Drawing.java             # Drawing interface
├── LocatedRectangle.java    # Positioning interface
│
├── Body.java                # Body component
├── Head.java                # Head component
├── Eyes.java                # Eyes component
├── Mouth.java               # Mouth component
├── Neck.java                # Neck component
├── Horns.java               # Horns component
├── Legs.java                # Legs component
├── Tail.java                # Tail component
│
├── SpringbokDecorator.java  # Base decorator
├── HatDecorator.java        # Adds a hat
├── ShoesDecorator.java      # Adds shoes
├── SingingDecorator.java    # Adds singing behavior
├── FaceColorDecorator.java  # Changes face color
│
├── Accessory.java           # Enum for accessories/behaviors
├── AudioPlayer.java         # Plays WAV audio
├── RandomNumber.java        # Utility for random values
└── singing.wav.wav          # Audio file for singing
```

## Design Patterns

- **Decorator Pattern** — Accessories (hat, shoes, singing) are applied as decorators wrapping the base `Springbok` object.
- **Interface-based design** — `Animal`, `Drawing`, and `LocatedRectangle` define clean contracts for components.

## How to Run

### Requirements
- Java 8 or higher
- An IDE like Eclipse, IntelliJ, or VS Code with Java support

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/khoya1/Springbok.git
   ```
2. Open the project in your IDE.
3. Run `DrawingTool.java` as a Java application.

## Screenshots

> Add a screenshot here once running!

## License

This project was created as a learning exercise. Feel free to use and adapt it.
