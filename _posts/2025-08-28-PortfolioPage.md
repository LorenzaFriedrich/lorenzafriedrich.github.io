---
title: Lorenza Friedrich's Portfolio (Start Here)
date: 2025-08-28 13:19:00 +0800
categories: [Personal Projects, Portfolio]
tags: [unity, unreal engine, arduino]     # TAG names should always be lowercase
description: Portfolio of work I can share with recruiters and interested parties 
pin: true
---

# Welcome to my Portfolio! 

### Projects

#### 3D Third-Person Delivery Game (Unity) - GoreDash

![alt text](../assets/img/GoreDash/pickup.gif)

Developed with a four-person team, this project challenges players to complete timed deliveries across a city while avoiding enemy rats and robbers. Players follow a dynamic waypoint system, manage health and time, and use collectibles to survive.

##### Main Menu

<video controls src="../assets/img/GoreDash/MineandNookInc_GoreDash - Intro.mp4" title="Title"></video>

##### Level Play Through 
<video controls src="../assets/img/GoreDash/MineandNookInc_GoreDashLevelplay.mp4" title="Title"></video>

Core Features: Pickup & delivery system, level progression, dynamic waypoint arrow, HUD with health/timer/objectives, start/pause menus, options (volume, restart, game over), and loading screens.

Collectibles: Health packs (restore health), speed boosts (temporary movement increase), pepper spray (stuns rats for 10 seconds).

Enemies: Rats: AI-controlled with chase, patrol, and idle states; damage on contact; can be stunned. Robbers: Target the delivery box; chase when carried; steal package on contact and reset it to start; also damage the player.

Player Abilities: Running, picking up/delivering packages, using collectibles for survival and strategy.

#### PSI Lisp Interpreter in C

My Lisp interpreter takes an input in the terminal from a user and returns a computation. It takes in numbers, booleans, symbols, lists, functions, definitions, heads/tails/cons, quotes (WIP), strings, inputs/outputs, and types. Examples below: 
```c
psi> (+)
0
psi> (+ 5 6 7)
18
psi> (= 3 3 4)
#f
psi> (< 3 4 5)
#t
psi> (not #t)
#f
psi> (not 1)
#f
psi> (not #f)
#t
psi> (= 0 ()) 
#f
psi> (!= 0 ())
#t
psi> (def a 7) 
7
psi> a
7
psi> (+ a 4)
11
psi> (def a (+ a 6)) 
13
psi>  (+ a 4) 
17
psi> (+ 3 4) 
7
psi> (/ 1 0)
$error{(Divide by zero)}
Evaluation failed.
psi> (+ _ 1)
8
psi> (def l (cons 1 (cons 2 ())))
(1 2)
psi> (head l)
1
psi> (tail l)
(2)
psi> (quote x)
x
psi> 'x
x
psi> "cat"
"cat"
psi> (ord "cat")
(99 97 116)
psi> (input)
hello
"hello"
psi> (output "Hello\n\nworld!\n")        
Hello\n\nworld!\n
#t
psi> (type #t)
bool
psi> (type 1)
num
```

More information on Intro to C Post

#### Unreal Engine - Rube Goldberg Machine (In Progress)



#### Frogget - Arduino Pixel Chix Project (In Progress)

### Skills


#### Note
Due to Georgia Institute of Technology's strict policies around sharing code and my previous job's policies around sharing proprietary work, I can't share github repositories easily, nor a majority of my accomplishments. This page is my best attempt to showcase my skills in a way that is easily accessible for recruiters/interested parties. 


