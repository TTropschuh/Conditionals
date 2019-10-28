# Conditionals and Coordinates

## The bouncing ball

```javascript

let ballX = 0;
let ballY = 0;
let ballXSpeed = 2.5;
let ballYSpeed = 1;
let ballColorR = 0;
let ballColorG = 0;
let ballColorB = 0;

function setup() {
    createCanvas(400, 400);
    ballX = width / 2;
    ballY = height / 2;
}

function draw() {
    //background(255);
    drawBall(ballX, ballY);
    ballX += ballXSpeed;
    ballY += ballYSpeed;

    if (ballX < 0 || ballX > width) {
        ballXSpeed = ballXSpeed * -1;
      ballColorR = random (0, 255);
      ballColorG = random (0, 255);
      ballColorB = random (0, 255);

    }
    if (ballY < 0 || ballY > height) {
        ballYSpeed = ballYSpeed * -1;
      ball

    }

}

function drawBall(bx, by, size = 25) {
    noStroke();
    fill(ballColorR, ballColorG, ballColorB);
    circle(bx, by, size);
}

```
## The cross
```javascript

let stripspeed = 2.5;

function setup() {
  createCanvas(400, 400);
  angleMode(DEGREES);
}

function draw() {
  // draw the frame
  background("#E6E0E2");
  stroke("#887987");
  noFill();
  rectMode(CENTER);
  rect(width / 2, height / 2, width * 0.86, height * 0.86);

  push()
  translate(width / 2, height / 2);
  stroke("#9D2D35");
  let posx1 = -100;
  let posx2 = 100;
  let posy1 = 0;
  let posy2 = 0;
   rotate(45);
  line(posx1, posy1, posx2, posy2);
  rotate(90);
  line(posx1, posy1, posx2, posy2);

  pop()

}
```

## Make sketch 2 fancy

Didn't manage...yet. :/
