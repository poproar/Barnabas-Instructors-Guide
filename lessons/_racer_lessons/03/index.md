---
layout: lesson
title: Lesson 3 &middot; Introducing Inputs

suggested_time: 60-75 minutes  

disciplines:
    - "Define a simple design problem that can be solved through the development of an object, tool, process, or system and includes several criteria for success and constraints on materials, time, or cost. (3-5-ETS1-1)"

technical_skills:
    - Wish we had a standard list
life_skills:
    - Item

essential_questions: 
    - Good Questions?

vocab:
    - Word

videos:
    - link: https://youtu.be/ZEVIdkZvHmQ
      text: The Button LED Circuit 
    - link: https://youtu.be/-UxbsqI5vh0
      text: Wiring the Button and LED for programming
    - link: https://youtu.be/VlEWea9keUY
      text: Programming the Button with Ardublock 
      
documents:
    - link: https://docs.google.com/document/d/1RjIKehsaCcfTbdf2GcppbJY5CQgtfXmkB68EUZ575ao/edit
      text: Wiring Your Button
    - link: https://docs.google.com/document/d/1TY2-oVnaUzFOpudlrqpmC8Ye1gYToZ9KbVqL1nooPwk/edit
      text: Wiring The Button as an Input
other:

barriers: 
    - Minimal understanding of 

anticipatory:
    - Make them excited to learn

practice:
    - independence

assessment:
    - affirmation of understanding

materials:
    - Engineering Journal

reflection:
    comprehension:
      - What are we assessing?

---

#### Review
   * Previous week  
   * Critical think based on previous question

### Step 1: First Button Circuit (15 minutes) 
In order to use your button, you need to tell your Barnabas Noggin to do something IF it is pushed.  
How do you do that?

#### Button Schematic
![fig 3.1](fig-3_1.png){:class="image "}

- Using the breadboard, wires, button and LED, build the circuit above.
- First remove all your wires from your robot.
- Next, place the button onto your bread board (see below).  Make sure to that the button is turned the right way!

![fig 3.2](fig-3_2.png){:class="image "}

- Now add the resistor and the LED.
  - HINT: Row 1 should be connected to the "-" of the LED.
  - HINT: Row 3 should be connected to GND.
- Once you are done, power up the noggin by connecting the USB.  Your LED should only turn on if you push the button down.  If it's not working correctly, double check your circuit! 
- The final circuit should look something like this;

![fig 3.3](fig-3_3.png){:class="image "}


### Step 2: Wiring the Button as Input (15 minutes) 
#### Schematic
![fig 3.4](fig-3_4.png){:class="image "}

- Now we will wire your button to pin 2 so that our Barnabas Noggin can sense when you have pushed it. 
- Build the circuit above!
- The final product should look similar to this;

![fig 3.5](fig-3_5.png){:class="image "}

### Step 3: Programming the Buton (15 minutes) 
#### Introduction to Inputs
##### as Blocks
###### Conditional Logic
We want to the light to turn ON if we press the button and turn OFF if we let go of the button.  We’ll need a new block.  See below!
![fig 3.6](fig-3_6.png){:class="image "}

The above block is used to check whether the button has been pressed and act accordingly. In the following code it is crucial to getting the behavior we are looking for;
![fig 3.7](fig-3_7.png){:class="image "}
Create this code yourself and try it out!

{% include youtube.html id='VlEWea9keUY' %}
[Programming the Button with Ardublock](https://youtu.be/VlEWea9keUY).

##### as Text
In order to use your button, you need to tell your Barnabas Noggin to do something IF it is pushed.  How do you do that?  
Here, we will learn about a few new commands

Now we want to the light to turn ON everytime I press the button and turn OFF every time I let go of the button.  You'll need to use a new conditional function called if/else. See below;

```
void setup()
{
  pinMode( 2 , INPUT);
  pinMode( 7 , OUTPUT);

}

void loop()
{
  if (digitalRead(2) == HIGH) {
    digitalWrite(7,LOW);
  }
  else {
    digitalWrite(7,HIGH);
  }
}
```

{% include youtube.html id='OA2PoLzCDMI' %}
[Programming The Button and LED with Arduino IDE](https://youtu.be/OA2PoLzCDMI)

#### Extra Challenges
Now that you know how to program a button, try the following challenges:  

1. Modify your program so that it blinks 5 times and then turns off whenever you push the button.
2. Try adding the buzzer to your circuit (pin 6) and make it buzz only if the button is pushed.
3. Try having the button blink 5 times only if you push the button twice.

{% include badge.html type='best_practice' content="notes from today's lesson 3 class. - it worked well to have the students log in to schoology and walk through all the connections together as a class - we should add the led circuit to the diagram as well - add a note about squeezing the button so that it doesn't take up 4 rows. you want it to take up 3 rows - the way the button needs to be oriented on the breadboard is tricky. this is something that we need to think about - after wiring was confirmed, it was good to have the students figure out how to copy the ardublock program to program their first sensing program - we only got to worksheet 2 in our 55 min class. The whole lesson would probably take 1.5 hrs. - it was good to go over what is now possible using the switch. I explained pseudo code and states of the circuit.. add this to the lesson plan curriculum" %}

{% include badge.html type='suggestion' content='Challenges for kids who do not have entire robot wired up. 1) have the light flash 3 times when you press the button and then turn off 2) have the light turn on when you push the button and have it turn off when you let go.' %}