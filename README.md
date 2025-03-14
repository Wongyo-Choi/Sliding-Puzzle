# Sliding Puzzle

A Java-based sliding puzzle game demonstrating essential game logic, graphical user interface (GUI) design, and unit testing. The source code is organised within the `uk.ac.man.cs.puzzle` package.

## Overview

The sliding puzzle is a classic brain teaser that challenges players to arrange tiles into the correct order by sliding them around one empty space. This project utilises Java for both logic and GUI components, with JUnit providing testing support.

## Project Structure

```
sliding-puzzle
├── lib
│   ├── java-hamcrest-2.0.0.0.jar
│   └── junit-4.12.jar
├── src
│   └── uk/ac/man/cs/puzzle
│       ├── gui
│       │   ├── GUI.java
│       │   └── GraphicsPanel.java
│       └── logic
│           ├── Model.java
│           └── Tile.java
├── test
│   └── uk/ac/man/cs/puzzle
│       ├── gui
│       └── logic
│           ├── MouseInteractionTest.java
│           └── ValidMovementTest.java
├── build.xml
└── README.md
```

- **lib**: External libraries (JUnit and Hamcrest) for unit testing.
- **src**: Main source files:
  - **gui**: Contains classes for the graphical user interface (`GUI.java` and `GraphicsPanel.java`).
  - **logic**: Houses the puzzle’s logic (`Model.java` and `Tile.java`).
- **test**: Includes JUnit test classes for both GUI and logic.
- **build.xml**: Ant build script for compiling, testing, and running.

## Requirements

- Java Development Kit (JDK) 1.8 or later
- Apache Ant (for build and test tasks)
- JUnit 4.12 (in `lib`)
- Hamcrest 2.0 (in `lib`)

## Building and Running

1. **Compile**  
   From the project’s root directory, run:
   ```bash
   ant compile
   ```
   This compiles the source code in `src`.

2. **Test**  
   Execute:
   ```bash
   ant test
   ```
   This runs the JUnit tests located in `test`.

3. **Run**  
   Launch the puzzle application:
   ```bash
   ant run
   ```
   This displays the sliding puzzle GUI.

## Usage

Once running, the GUI presents a grid of tiles with one empty space. Move the tiles into their correct positions by clicking or using the keyboard (implementation may vary). The puzzle is solved when all tiles are in the correct order.

## Customisation

- **Board Size**: Modify the puzzle dimensions in `Model.java` for various grid sizes (e.g., 3×3, 4×4, 5×5).
- **Graphics**: Update drawing methods or replace images in `GraphicsPanel.java` to change the puzzle’s appearance.
- **Input Handling**: Adapt `GUI.java` or `GraphicsPanel.java` for different input devices or custom controls.

## References

- [Java Official Documentation](https://docs.oracle.com/en/java/)
- [JUnit Documentation](https://junit.org/junit4/)
- [Wikipedia: 15 Puzzle](https://en.wikipedia.org/wiki/15_puzzle)
