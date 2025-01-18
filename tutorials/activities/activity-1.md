# Brick Breaker


## Introduction @unplugged

**Let's make the classic Brick Breaker Game!**

In this tutorial, you'll create the paddle, and make it move!

---
![Game Demo](https://github.com/OkanaganCodeAcademy/brick-breaker-skillmap/blob/main/tutorials/images/brick-breaker-game-demo.gif?raw=true "Game Demo")



## Creating the Paddle 

Lets start by making the Paddle Sprite!

- :paper plane: Open ``||sprites:Sprites||`` and drag ``||variables:set sprite to||`` *to the bottom* of the ``||loops:on start||``.
- :mouse pointer: Click on ``||variables: mySprite||`` and select the ``||variables: Rename||`` option 
and rename the sprite to **paddleSprite**.

![Rename Sprite](https://github.com/OkanaganCodeAcademy/brick-breaker-skillmap/blob/main/tutorials/images/brick-breaker-rename-sprite.gif?raw=true "Rename Sprite")

---


## Changing the Sprite Kinds

The game needs to know how we want our sprites interact and Sprite Kinds are key to making our game work the way we expect. So let's change the Paddle's Sprite Kind!


- :mouse pointer: Click on ``||sprites: Player 🔽||`` and select the ``||sprites: Add a new Kind||``.
Lets name it **Paddle**.

**insert gif adding new Sprite Kind**
- :mouse pointer: Next click the gray box to create the paddle. **Note:** A good size for the paddle is 20 pixels wide, and 3 pixels tall.

**insert gif of clicking on grey box then setting the size**

---

## Setting the Position

Uh-oh, our paddle is in the middle of the screen! That may make it difficult to play the game!
To fix this, we need to position the paddle near the bottom of the screen.

- :paper plane: To set the paddle's position drag out the  ``||sprites:set sprite position||`` and *place it beneath* the paddle sprite.
**Caution:** make sure the name in the ``||sprites:set sprite position||`` block matches the sprite name we chose earlier!
- :mouse pointer: Set the ``||sprites:x||`` value to `80` and ``||sprites:y||`` value to `115`
---

### Knowledge Check
- What do the ``||sprites:x||`` and ``||sprites:y||`` values represent?
---

## Moving the Paddle with buttons

Now lets make the paddle move!

**insert gif of paddle moving**

- :game: Open ``||controller:Controller||`` and drag out the ``||controller:move sprite with buttons ⊕||`` into ``||loops:on start||`` beneath all our other code!
**Caution:** make sure the name in the ``||controller:move sprite with buttons ⊕||`` block matches the sprite name we chose earlier!
- :mouse pointer: Next click on the ``||controller: ⊕||`` to open up the **Velocity Parameters**. 
Since we only want our paddle to move left and right we need to set the vertical velocity parameter ``||controller:vy||`` to `0`

---


### Knowledge Check
- What is Velocity?
- What is a Parameter?
- What do the ``||controller:vx||`` and ``||controller:vy||`` values represent?
- What if we set ``||controller:vx||`` to `-50`?
---


## Play Test

Playtest your game! Do you notice any issues? 
What about when your paddle reaches the edge of the screen?

**insert play testing gif**

---

## Staying in-screen

Oh no! The Paddle leaves the screen may make it difficult to play the game! Let's fix it.

- :paper plane: Open ``||sprites:Sprites||`` and drag out the ``||sprites: set sprite stay in screen ||`` and place it *at the bottom* of the ``||loops:on start||``
and select the name **paddleSprite**

---

## On to the next one!
### 🎊 Congratulations! 🎊
Just like that you have the first piece of your Brick Breaker game! Keep up the amazing work 😄
