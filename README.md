# SinkShip AI tester

## Interactive test

### Usage:

```python tester.py http://<your-ip>:<port>/make-move```

It will start an interactive game where you are able to see your AI's progress each round:

### Example
```
$ python tester.py http://localhost:8080/make-move

Round 1: AI shoots at x: 0 and y: 1
? ? ? ? ? 
X ? ? ? ? 
? ? ? ? ? 
? ? ? ? ? 
? ? ? ? ? 

Press enter to shoot again (ctrl+c to exit)

Round 2: AI shoots at x: 0 and y: 0
~ ? ? ? ? 
X ? ? ? ? 
? ? ? ? ? 
? ? ? ? ? 
? ? ? ? ? 

Press enter to shoot again (ctrl+c to exit)

Round 3: AI shoots at x: 0 and y: 2
~ ? ? ? ? 
X ? ? ? ? 
~ ? ? ? ? 
? ? ? ? ? 
? ? ? ? ? 

Press enter to shoot again (ctrl+c to exit)

Round 4: AI shoots at x: 1 and y: 1
~ ? ? ? ? 
2 2 ? ? ? 
~ ? ? ? ? 
? ? ? ? ? 
? ? ? ? ? 

Press enter to shoot again (ctrl+c to exit)

Round 5: AI shoots at x: 3 and y: 0
~ ? ? ~ ? 
2 2 ? ? ? 
~ ? ? ? ? 
? ? ? ? ? 
? ? ? ? ? 

Press enter to shoot again (ctrl+c to exit)

Round 6: AI shoots at x: 2 and y: 2
~ ? ? ~ ? 
2 2 ? ? ? 
~ ? ~ ? ? 
? ? ? ? ? 
? ? ? ? ? 

Press enter to shoot again (ctrl+c to exit)

Round 7: AI shoots at x: 1 and y: 2
~ ? ? ~ ? 
2 2 ? ? ? 
~ X ~ ? ? 
? ? ? ? ? 
? ? ? ? ? 

Press enter to shoot again (ctrl+c to exit)

Round 8: AI shoots at x: 1 and y: 3
~ ? ? ~ ? 
2 2 ? ? ? 
~ X ~ ? ? 
? X ? ? ? 
? ? ? ? ? 

Press enter to shoot again (ctrl+c to exit)

Round 9: AI shoots at x: 1 and y: 4
~ ? ? ~ ? 
2 2 ? ? ? 
~ 1 ~ ? ? 
? 1 ? ? ? 
? 1 ? ? ? 


AI sank all ships in 9 moves!
```

## Stress test

### Usage:

```python tester.py http://<your-ip>:<port>/make-move stress```

It will fire 100 game boards at your AI and calculate an avarage

### Example

```
$ python tester.py http://localhost:8080/make-move stress
Game 1 done in 19 rounds
Game 2 done in 21 rounds
Game 3 done in 13 rounds
Game 4 done in 19 rounds
Game 5 done in 21 rounds
Game 6 done in 9 rounds
Game 7 done in 13 rounds
Game 8 done in 16 rounds
Game 9 done in 9 rounds
Game 10 done in 13 rounds
Game 11 done in 10 rounds
Game 12 done in 15 rounds
Game 13 done in 7 rounds
Game 14 done in 12 rounds
Game 15 done in 14 rounds
Game 16 done in 13 rounds
Game 17 done in 13 rounds
Game 18 done in 17 rounds
Game 19 done in 16 rounds
Game 20 done in 9 rounds
Game 21 done in 7 rounds
Game 22 done in 14 rounds
Game 23 done in 19 rounds
Game 24 done in 14 rounds
Game 25 done in 13 rounds
Game 26 done in 19 rounds
Game 27 done in 22 rounds
Game 28 done in 14 rounds
Game 29 done in 16 rounds
Game 30 done in 10 rounds
Game 31 done in 15 rounds
Game 32 done in 11 rounds
Game 33 done in 15 rounds
Game 34 done in 15 rounds
Game 35 done in 17 rounds
Game 36 done in 7 rounds
Game 37 done in 14 rounds
Game 38 done in 19 rounds
Game 39 done in 16 rounds
Game 40 done in 17 rounds
Game 41 done in 17 rounds
Game 42 done in 10 rounds
Game 43 done in 18 rounds
Game 44 done in 16 rounds
Game 45 done in 12 rounds
Game 46 done in 8 rounds
Game 47 done in 18 rounds
Game 48 done in 17 rounds
Game 49 done in 13 rounds
Game 50 done in 15 rounds
Game 51 done in 16 rounds
Game 52 done in 15 rounds
Game 53 done in 6 rounds
Game 54 done in 20 rounds
Game 55 done in 9 rounds
Game 56 done in 23 rounds
Game 57 done in 10 rounds
Game 58 done in 18 rounds
Game 59 done in 6 rounds
Game 60 done in 8 rounds
Game 61 done in 23 rounds
Game 62 done in 16 rounds
Game 63 done in 16 rounds
Game 64 done in 12 rounds
Game 65 done in 21 rounds
Game 66 done in 12 rounds
Game 67 done in 15 rounds
Game 68 done in 16 rounds
Game 69 done in 17 rounds
Game 70 done in 9 rounds
Game 71 done in 9 rounds
Game 72 done in 11 rounds
Game 73 done in 10 rounds
Game 74 done in 16 rounds
Game 75 done in 18 rounds
Game 76 done in 11 rounds
Game 77 done in 17 rounds
Game 78 done in 19 rounds
Game 79 done in 14 rounds
Game 80 done in 19 rounds
Game 81 done in 14 rounds
Game 82 done in 15 rounds
Game 83 done in 16 rounds
Game 84 done in 10 rounds
Game 85 done in 13 rounds
Game 86 done in 9 rounds
Game 87 done in 11 rounds
Game 88 done in 14 rounds
Game 89 done in 12 rounds
Game 90 done in 9 rounds
Game 91 done in 17 rounds
Game 92 done in 15 rounds
Game 93 done in 19 rounds
Game 94 done in 16 rounds
Game 95 done in 13 rounds
Game 96 done in 15 rounds
Game 97 done in 20 rounds
Game 98 done in 10 rounds
Game 99 done in 8 rounds
Game 100 done in 7 rounds

Total rounds 1412 in 100 games

Avarage of 14 per game
```