---
layout: page
title: Snakes and Ladders Game
description: A Python implementation of the classic Snakes and Ladders game using Turtle graphics.
img: assets/img/Snake.jpg
importance: 3
category: Fun
---

Welcome to the world of our "Snakes and Ladders Game" project, a Python implementation of the classic board game using the Turtle graphics library.

**Snake & Ladder** is a "Turtle" based user-friendly game. Turtle is a pre-installed Python library that allows you to command the turtle to draw all over it! Each turtle pointer has a unique identity as a player's piece. The turtle screen resembles a graph sheet, and each point on the screen has individual coordinates.

The core of the game relies on Python's associative arrays, known as dictionaries. The dictionaries store information in the form of key-value pairs, where the block number is the key, and the coordinates of the block number are its corresponding value. Randomization is achieved through the Python "random" library, ensuring that rolling a die is an independent event with numbers in the range of one to six.


## How to Play

1. The game has two game pieces - YELLOW and BLUE. YELLOW uses the 'Down' arrow key to roll the dice, while BLUE rolls by using the 'Up' arrow key.
2. The first move is played by YELLOW. Players take turns rolling the dice and moving their pieces ahead. Unintentional wrong arrow key presses will not affect the game.
3. There is no double chance on impressive numbers, such as (6,1).
4. The player who crosses square 30 first wins the game.
5. If a player's piece lands on the lower-numbered end of a ladder, the player moves the token up to the ladder's higher-numbered square. If the player lands on the higher-numbered square of a snake, the token must be moved down to the snake's lower-numbered enclosure.


## Contributions

Contributions are welcome! If you have ideas for improvements, new features, or want to collaborate on the project, feel free to fork the repository and create a pull request.

## License

This project is open-source and available under the MIT License.

## Acknowledgments

Special thanks to the creators of the Python Turtle graphics library for making it fun to visualize the game.

Enjoy playing the Snake & Ladder Game!
   
    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---
<!-- 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Snake.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div> -->
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Snake.jpg" title="Game BG" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The game is based on sheer luck, and each player has an equal probability of winning.
</div>


<div class="row">
    <div class="col-sm">
        <iframe width="100%" height="315" src="https://www.youtube.com/watch?v=bjgOrAyTI5A" frameborder="0" allowfullscreen></iframe>
    </div>
</div>
<div class="caption">
    Learn more about the project by watching our video tutorial. It provides a step-by-step guide on how to play the game and an inside look at its development.
</div>



<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %}



