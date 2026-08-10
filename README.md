Breakout++

Breakout++ is a small fan-made Breakout-style arcade game written in C++ using raylib.

The goal is simple: move the paddle, keep the ball in play, and destroy the wall of bricks.

Disclaimer

This project is an unofficial, fan-made clone inspired by the classic Breakout game.

I am not affiliated with, endorsed by, sponsored by, or associated with Atari in any way.Atari and Breakout are trademarks and/or properties of their respective owners.

This project was created for learning, programming practice, and non-commercial hobby use.

Current Features

C++ game code built with raylib

1280 × 800 game window

60 FPS target

Paddle movement with the left and right arrow keys

Ball movement and wall bouncing

Paddle collision

Brick collision

40 bricks arranged in an 8 × 5 grid

Five colored brick rows

3-life system

Ball reset after losing a life

Press Enter to launch after a life is lost

Simple programmatically drawn graphics

Controls

Key

Action

Left Arrow

Move paddle left

Right Arrow

Move paddle right

Enter

Launch / resume the ball

Window close button

Exit the game

Gameplay

When the game starts, press Enter to launch the ball.

Use the paddle at the bottom of the screen to keep the ball from falling out of bounds. When the ball hits a visible brick, the brick disappears and the ball changes vertical direction.

You begin with 3 lives. If the ball reaches the bottom of the screen, one life is removed and the ball is reset.

Brick Layout

The current level contains an 8 × 5 grid of bricks:

R R R R R R R R

O O O O O O O O

Y Y Y Y Y Y Y Y

G G G G G G G G

B B B B B B B B

Each row uses a different color:

Red

Orange

Yellow

Green

Blue

Project Structure

.
├── ball.cpp
├── ball.h
├── bricks.cpp
├── bricks.h
├── paddle.cpp
├── paddle.h
├── main.cpp
└── .gitignore

ball.cpp / ball.h

Handles:

Ball position

Ball velocity

Drawing

Screen-edge collisions

Lives

Ball reset behavior

Paddle collision workaround

bricks.cpp / bricks.h

Handles:

Creating the brick grid

Brick positions

Brick visibility

Brick colors

Drawing bricks

Detecting ball-to-brick collisions

paddle.cpp / paddle.h

Handles:

Left/right keyboard input

Paddle velocity

Keeping the paddle on screen

Drawing the paddle

main.cpp

Contains the main game loop and connects the ball, paddle, and brick systems.
