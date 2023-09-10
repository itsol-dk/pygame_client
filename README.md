# pygame_client
Client for the pygame

### Import the challenge game (make sure that you are in the same folder)
```python
import challenge
```
### Connect to the game server
```python
game=challenge.client(ip_address=IP, port=PORT_NO)
```
### Login 
```python
game.login("test1234","testensen")
```

### Get the first question
```python
game.question(0)
```
### Get the data for the first question
```python
game.data(0)
```
### Lets create a function that returns the data
```python
def my_answer0(my_var):
    return my_var
```
### Lets submit our answer
```python
game.answer(0,my_answer0(game.data(0)))
```

It will tell you right away whether the answer is right or wrong
You can at any point see the score by calling 

```python
game.score()
```
