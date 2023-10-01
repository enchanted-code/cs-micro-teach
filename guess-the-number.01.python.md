# Guess The Number

## Syntax Recap
<!-- Get brain thinking about previous acquired knowledge -->
Here's a reminder of some of the syntax found in Python.

| Code                   | Description                                           |
|:-----------------------|:------------------------------------------------------|
| `print("Hello World")` | Output Message To Screen                              |
| `stuff = input("?")`   | Request User Input With Message And Store In Variable |
| `foo = ...`            | Define a variable                                     |
| `if ... elif ... else` | Create Logic                                          |
| `while ...`            | Iteration With While Loop                             |
| `for ...`              | Iteration With For Loop                               |

## Goal/Plan
<!-- Give clear objective, English context to code -->
- Computer generates random number for user to guess, let's say between 1 and 10
- Keeps asking user for guess input until answer is correct
    - Hints if users guess is too high or low
- When answer is correct ends the game with a friendly message

## Construct The Program
<!-- Whole class interaction, without needing to remember exact syntax, focusing on logical reasoning -->
How can we construct the program using these lines of code?

1. `import random`
2. `users_guess = int(users_guess)`
3. `users_guess = None`
4. `while users_guess != generated_guess:`
5. `generated_guess = random.randint(1, 10)`
6. `print("Guess The Number Game")`
7. `print("You Guessed To High")`
8. `print("You Guessed To Low")`
9. `users_guess = input("Enter Your Guess (1-10): ")`
10. `if users_guess > generated_guess:`
11. `print("You guessed correct!")`
12. `elif users_guess < generated_guess:`

<details>
<summary>Solution</summary>

```python
import random

print("Guess The Number Game")

generated_guess = random.randint(1, 10)

users_guess = None

while users_guess != generated_guess:
    users_guess = input("Enter Your Guess (1-10): ")

    users_guess = int(users_guess)

    if users_guess > generated_guess:
        print("You Guessed To High")

    elif users_guess < generated_guess:
        print("You Guessed To Low")

print("You guessed correct!")
```

</details>

## Let's Test It!
<!-- Did we get anything wrong? What happens? -->
Now the program is complete, let's see if it runs.

## Expanding Game?
<!-- Thinky think time and some creativity, also see if they can relate ideas to actually programming it for later... -->
How can we make this game more fun and possibly add a greater challenge?

<details>
<summary>Possible Ideas</summary>

- limit number of guesses allowed
- ask user if they want to play again
- a way of exiting mid game
- allowing user to enter min/max of generated number

</details>

## What Did We Learn?
<!-- Check understanding of techniques used -->
- Write some short bullet-points on what was used and why
    - e.g. "random" was imported so we could generate random numbers between a given range
- Then share some with the class
