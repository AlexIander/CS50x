# CS50x
Progress in my CS50x class

Currently working on the Scratch editor

In Ghost Attack, I have built a basic "Stop the Boats" clone. 
The last thing I need is to figure out a way to get the ghost to spawn far away from the centre.

I can get it to appear anywhere between -260<x<260 and -260<y<260 but the trouble lies in that it can spawn at (0,0) for an instant life loss.
I need a way to generate random positive and negative numbers without hitting (0,0)

I've solved the spawn problem. 
Essentially what I wanted was the ghosts to spawn on a big square outside the field of view.
So instead of trying to create the square all at once, I split up the problem into the four side of the square

So (x,y) becomes (-260, -260<y<260), (260, -260<y<260), (-260<x<260, -260), (-260<x<260, 260)
And just a random number generator to pick between the 4

Now the ghost will not spawn too close (or directly on) the centre and break the game.

And I have submitted my Problem Set 0.
Because arrays start at zero.
