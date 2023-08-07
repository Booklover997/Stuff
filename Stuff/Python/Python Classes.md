#python 

[[Method]]s are used to execute functions on a particular object.
Used to created templates that can be used to create objects with different attributes. self is used to refer to variables housed in the class.

___

\_\_init_\_ allows for variables to assigned as the object is created
```python
def __init__(self, var1, var2):
	self.var1 = var1
	self.var2 = var2
```


An example her monster game made 7/15/2023 for #CyberFoundations
```python
import random
import sys
class Hero():
    health = 100
    damage = 25
    potions = 1
    def __init__(self, health, damage ):
        self.health =health
        self.damage = damage
        self.potions =1
    def attack(self, enemy):
        enemy.receiveDamage(self.damage)
    def receiveDamage(self, damage):
        self.health  -= damage
        if self.health <= 0 :
            print("You Have Lost")
    def heal(self):
        if self.potions > 1 :
            self.potions -=1
            health +=5

class Monster():
    health = random.randint(1,25)
    damage = random.randint(1,100)
    def __init__(self, health, damage):
        self.health = health
        self.damage = damage
    def attack(self, enemy):
        enemy.receiveDamage(self.damage)
    def receiveDamage(self, damage):
        self.health  -= damage
        if self.health == 1:
            print("The monster has ran away!")
        if self.health <1:
            print("The monster has died!")
    def roar(self):
        pass
Hero(sys.argv[1], sys.argv[2])
Monster(random.randint(1,100), random.randint(1,25))
while Hero.health > 0 and Monster.health>1:
    Hero.attack(Monster)
    Monster.attack(Hero)
print("The end")
```
