# Airplane Battle Game

This is a 2D airplane shooting game based on Java, supporting both single-player mode and online multiplayer mode. Players can control the airplane to move, shoot enemies, and collect reward items to achieve higher scores.

## Features

- Single-player game mode  
- Online multiplayer battle mode  
- Stunning game interface and sound effects  
- Real-time collision detection  
- Score management system  
- Game save functionality  

## Technology Stack

- Java 8+  
- Java Swing  
- Java Socket Programming  
- MySQL database  
- Maven build tool  

## Directory Structure

```
src/
├── main/
│   ├── java/
│   │   └── com/ex/airplane/ - Java source code
│   │       ├── GameObject/ - Base classes and implementations of game objects
│   │       ├── UI/ - User interface components
│   │       ├── multiplayer/ - Classes related to multiplayer mode
│   │       ├── Server/ - Game server implementation
│   │       ├── AudioPlayer.java - Audio player
│   │       ├── CollisionHandler.java - Collision detection handler
│   │       ├── Main.java - Game startup class
│   │       └── ScoreManager.java - Score manager
│   │
│   └── resources/ - Resource files
│       ├── BGM.wav - Background music
│       ├── bullet.png - Bullet image
│       ├── enemy.png - Enemy airplane image
│       ├── explosion.wav - Explosion sound effect
│       ├── player.png - Player airplane image
│       └── reward.png - Reward item image
```

## Installation and Running

### Single-player Mode

1. Ensure Java 8+ and Maven are installed  
2. Clone the project to your local machine  
3. Build the project:  
   ```
   mvn clean package
   ```
4. Run the game:  
   ```
   java -jar target/example-proj-1.0.0.jar
   ```

### Multiplayer Mode

1. Ensure Java 8+, Maven, and MySQL are installed  
2. Create a database in MySQL and import game.db  
3. Modify the database connection information in Server.java  
4. Build the project:  
   ```
   mvn clean package
   ```
5. Start the game server:  
   ```
   java -cp target/example-proj-1.0.0.jar com.ex.airplane.Server
   ```
6. Launch the client:  
   ```
   java -jar target/example-proj-1.0.0.jar
   ```

## Usage Instructions

- Use arrow keys to control airplane movement  
- Press the spacebar to fire bullets  
- Defeat enemies to earn points  
- Collect reward items for additional points  
- In multiplayer mode, you can play with other players  

## Contribution Guide

Contributions are welcome! Please follow these steps:

1. Fork the project  
2. Create a new branch  
3. Submit code changes  
4. Create a Pull Request  

## License

This project is licensed under the MIT License. For details, please refer to the LICENSE file in the project root directory.
