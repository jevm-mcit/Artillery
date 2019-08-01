# ARTILLERY
## Jack/Hack GAME

## instructions
Objective is to destroy enemy with ARTILLERY, user selects charge (1-10) and angle of fire in degrees (0-90) taking in consideration ground levels and wind.

Game ends when user has no more bombs

Each time a bomb destroys the enemy score is increased and two more bombs are added.

When game starts it prompts for a game number, this can be any number (or string) which is used to generate a seed for the random ground levels and wind generation.

## Implementation
Main.jack - Game runner with main() function
Game.jack - Main game controller, constructor prompts for game number
Projectile.jack - Simulates physics of projectile motion and draw it in screen, it Implements a very simple (Taylor series) trigonometric approximation for parabolic motion calculation (sin a = a, cos a = 1 - a² / 2, a in radians).  See https://en.wikipedia.org/wiki/Projectile_motion and https://en.wikipedia.org/wiki/Small-angle_approximation.  
Random.jack - Simple random number generation, see https://cdsmith.wordpress.com/2011/10/10/build-your-own-simple-random-numbers/
Ground.jack - Ground fields, randomly generates landscape

## Repo
https://github.com/jevm-mcit/Artillery
