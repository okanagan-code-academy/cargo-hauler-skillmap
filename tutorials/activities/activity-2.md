# Brick-Breaker Part 2

## Introduction @unplugged

**Let's make the ball for our Brick Breaker Game!**

In this tutorial, you'll create the ball, and make it move!

---

**insert gif of Brick-Breaker Game (Come from activity 1)**

## Creating the ball sprite

Lets start by making the Ball Sprite!

- :paper plane: Open `||sprites:Sprites||` and drag `||variables:set sprite to||` _to the bottom_ of the `||loops:on start||`.
- :mouse pointer: Click on `||variables: mySprite||` and select the `||variables: Rename||` option
  and rename the sprite to **ballSprite**.

**insert gif clicking and renaming the sprite**

---

## Changing the Sprite Kinds

The game needs to know how we want our sprites interact and Sprite Kinds are key to making our game work the way we expect. So let's change the Ball's Sprite Kind! (Comes from activity 1)

- :mouse pointer: Click on `||sprites: Player 🔽||` and select the `||sprites: Add a new Kind||`.
  Lets name it **Ball**.

**insert gif adding new Sprite Kind**

- :mouse pointer: Next click the gray box to create the ball. (Add a good size for the ball)

**insert gif of clicking on grey box then setting the size**

---

## Setting the Position

The **ballSprite** is in the middle of the screen! That may make it difficult to play the game once we add bricks!
To fix this, we need to position the ball near the lower half of the screen (but not below the paddle).

- :paper plane: To set the ball's position drag out the  ``||sprites:set sprite position||`` and *place it beneath* the **paddleSprite**.
  **Caution:** make sure the name in the ``||sprites:set sprite position||`` block matches the sprite name we chose earlier!
- :mouse pointer: Set the ``||sprites:x||`` value to `80` and ``||sprites:y||`` value to `90`

---

## Moving the Ball with velocity

Now lets make the ball move!

**insert gif of ball moving**

As you can see the ball is not moving. So, let's making it move.

- :paper plane: To set the ball's velocity drag out the `||sprites:set sprite velocity||` and _place it beneath_ the ball sprite.
  **Caution:** make sure the name in the `||sprites:set sprite velocity||` block matches the sprite name we chose earlier!
- :mouse pointer: Set the `||sprites:vx||` value to `50` and `||sprites:vy||` value to `50`.

---

### Knowledge Check

- What do the `||sprites:vx||` and `||sprites:vy||` values represent?

---

## Making ball bounce on walls

As we can see the ball is moving but it's going off the screen. So, let's fix it when it reaches the end of any screen then it will bounce of it.

- :paper plane: To set the ball to bounce on wall drag out the `||sprites:set sprite bounce on wall||` and _place it beneath_ the `||sprites:set sprite velocity||`.
  Make sure that it is set to ON!

---

### Knowledge Check (May need to change)

- What is Velocity?
- What is a Parameter?
- What do the `||controller:vx||` and `||controller:vy||` values represent?
- What if we set `||controller:vx||` to `-50`?

---

## Play Test

Playtest your game! Do you notice any issues?
**insert play testing gif**

---

## Events
- Coding **Event**s are things that happen in the system you are coding to help us determine how our code should react
- For example, we will use an Event to help decide when the **ballSprite** should bounce of the **paddleSprite**

### Sprites Overlap Event
- :paper plane: Open `||sprites:Sprites||` and drag `||sprites:On Sprites Overlap||` event block and place it somewhere where it does NOT overlap with other code blocks.
**Caution:** this code block does not attach to anything!

**insert dragging on sprites overlap block into code space gif**

---

## Setting Up the Event
- :mouse pointer: Click on the first `||sprites: Player 🔽||` and change it to `||sprites: Paddle||`
- :mouse pointer: Click on the second `||sprites: Player 🔽||` and `||sprites: Ball||`


## How do we get the ball to bounce?
- When a ball bounces off a something, it is simply changing the direction of it's motion.
- For example, if a ball is traveling downwards and hits a wall, it will bounce and then begin traveling upwards.
- In other words we are simply changing the direction of travel by multiplying the velocity-y (**vy**) by `-1`.
- The same is true about the x-direciton (left and right direction)!
**insert gif of ball bouncing off a top wall**

## Bouncing off the Paddle
The Paddle is like a bottom wall. A downwards travelling ball will hit the paddle, then bounce and begin travelling upwards!
- :paper plane: Open `||sprites:Sprites||` and drag `||sprites:set sprite x to||` block into the `||sprites:On Sprites Overlap||` Event block.
- :mouse pointer: Next, click on the `||sprites: x 🔽||` and select `||sprites: vy ||` from the dropdown menu.
- :calculator: Open the `||math:Math||` and drag out the `||math: 0x0||` and replace the `0` inside of the `||sprites:set sprite x to||` block.
- :paper plane: Next, open `||sprites:Sprites||` and drag the round `||sprites:Sprite x||` block. Replace a `0` in the `||math: 0x0||` block.
- :mouse pointer: Like before, click on `||sprites: x 🔽||` and select `||sprites: vy ||` from the dropdown menu.
- :mouse pointer: Finally, replace the other `0` with `-1`.
**insert image of completed block**



## On to the next one!

### 🎊 Congratulations! 🎊

Just like that you have the second piece of your Brick Breaker game! Keep up the amazing work 😄