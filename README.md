# pygame_client
Client for the pygame

### First start python in interactive mode
```python3```
### Import the challenge game (make sure that you are in the same folder)
### You can download the “challenge.py” file from fronter “Mandatory” -> “mandatory-part01-challenge”
```import challenge```
### Connect to the game server
```game=challenge.client(ip_address="IP",port=39594)```
### Login 
```game.login("test1234","testensen")```

### Get the first question
```game.question(0)```
### Get the data for the first question
```game.data(0)```
### Lets create a function that returns the data
```
def my_answer0(my_var):
    return my_var
```
### Lets submit our answer
```game.answer(0,my_answer0(game.data(0)))```
It will tell you right away whether the answer is right or wrong
You can at any point see the score by calling 
```game.score()```
