# Vectrex Pong

Tutorial: Programming a Pong game in C for the Vectrex, step by step.

![Pong: Programming Games in C for the Vectrex](assets/pong.gif)


## About

This tutorial teaches you how to program a complete Pong game for the
Vectrex console using C and the [VectreC](https://github.com/rogerboesch/vectreC)
toolchain (CMOC cross-compiler for 6809).

Each chapter builds on the previous one, gradually introducing core concepts
of Vectrex game development — from the game loop to collision handling and scoring.


## Chapters

| Chapter | Topic | File |
|---------|-------|------|
| 1 | The Game Loop | `src/tutorial1-chapter-01.c` |
| 2 | Initialising the Vectrex | `src/tutorial1-chapter-02.c` |
| 3 | Initialising your Game | `src/tutorial1-chapter-03.c` |
| 4 | Drawing Game Objects | `src/tutorial1-chapter-04.c` |
| 5 | Moving Game Objects | `src/tutorial1-chapter-05.c` |
| 6 | Adding the Game Logic | `src/tutorial1-chapter-06.c` |
| 7 | User Input — The Joystick | `src/tutorial1-chapter-07.c` |
| 8 | Game Object Interactions — Collision Handling | `src/tutorial1-chapter-08.c` |
| 9 | User Feedback — Scoring and Rewards | `src/tutorial1-chapter-09.c` |
| 10 | Final Version | `src/tutorial1-chapter-10.c` |
| 10+ | Final Version with Sound | `src/tutorial1-chapter-10-with-sound.c` |


## Prerequisites

Install the VectreC toolchain:

```bash
git clone https://github.com/rogerboesch/vectreC.git
cd vectreC
./build.sh
```

See the [VectreC README](https://github.com/rogerboesch/vectreC) for details.


## Building

Compile any chapter with:

```bash
VECTREC=$HOME/retro-tools/vectrec
$VECTREC/cmoc -I$VECTREC/stdlib -L$VECTREC/stdlib --vectrex -o pong.bin src/tutorial1-chapter-10.c
```


## Video Tutorial

Watch the full tutorial series on YouTube:

[Programming Games in C for the Vectrex](https://www.youtube.com/watch?v=m5Gxzj2xb2M&list=PLP6u_67PQGuHlz8J7U2Y6oUv05O_74D2w)


## References

* [VectreC toolchain](https://github.com/rogerboesch/vectreC) — CMOC cross-compiler for Vectrex
* [VIDE](https://github.com/malbanGit/Vide) — Vectrex IDE (recommended)
* [Vectrex Programming Tutorial (Assembler)](https://www.playvectrex.com/designit/chrissalo/toc.htm)
* [VectreC on Substack](https://vectrex.substack.com/p/vectrec) — Installation and usage guide


## License

Source code by Roger Boesch. Free to use, change and distribute.
