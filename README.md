# Online Reactable
## What is an Online Reactable?
<img align="left" src="readMeImages/MAE logo.png"  width="10%" style="margin-left:5px; margin-bottom:10px">
The Online Reactable is the recreation of a reactable on a web page that allows the user to create & combine sound waves, filters and effects in real time in an intuitive way. 

The original Reactable is an electronical musical instrument that lets the user create music by choosing buttons and putting them on an electronic table whose surface is a touch screen to change the effect parameters. Objects of oscillators and effects are selected and moved to generate a sound pattern, emulating the behavior of an analogue synthesizer. Parameters can be changed to obtain different kind of results and usually the production of music is accompanied by light effects. 

Our goal was to implement the physical Reactable on a web page so that it is more portable and accessible to all. The project has been developed for the course of Advanced Coding Tools and Methodologies for the Music and Acoustic Engineering Master’s degree of the Politecnico di Milano. 


## How does it work? 
The Online Reactable is made of a dark blue workspace interface surrounded by black columns that work as menus of oscillators, effects and filters. It is possible to include these buttons into the interface by clicking on them.

![Screenshot](readMeImages/interface.png)

The buttons can be subdivided in three categories: 
-oscillators, produces basic waveforms and and initiates the melody
-filters, which can alter the frequency composition of the sound
-effects, that can module sound and add reverb, tremolo, vibrato etc. 

Moreover, we included an envelope visulaizer and sliders on the top right part of the interface to visualize and modify the ADSR of the current synthiser envelope on the fly. 


## Buttons
The oscillators emit the melody playing notes with the timber of a specific kind of wave, while the filters cut the sound signals. It is possible to choose between the most common and used waves and filters so: 
- **sin, square, saw** and **triangle waves**
-**low, high** and **band pass filters.**
Every button is equiped with two knobs that let the user have control over the corresponding effect or sound.
The left one deals with the actual level or quality of the effect.
The right one regulates how "wet" the sound in output should be respect to the one in input.


## Envelope Regulator
The interface offers an option to alter the envelope parameters of the respective synths, via a visual interface in which the user can control the ADSR parameters on the fly.



## Movement and connecting lines
To obtain sound in output the user must create a connection between the melody makers and the output node, located at the very center of the workspace.
Every button is provided with connection nodes from which a line can be drawn. Oscillator nodes have one node for output while filters and effects have one input and one output. Creating a connection between buttons is easy: one must click on the output node of the first button and subsequently click the input node of the button to which the connection should arrive. To break the connection, it is enough to click again on the output node from which the line was created and the connection will vanish.


## Making music
If the user wishes to hear a melody with the unaltered sound from the oscillator he must connect the corresponding button directly to the output node, otherwise they can connect it to an effect and have this last one be connected to the general output. It is possible to have multiple in effects in cascade.
The user has control over several factors that include oscillator types, filters, and effects, and can combine and arrange them to obtain musical outputs with different sonic characteristics. The Web React table serves foremost as a tool for experimenting with musical timbre, textures and overall interesting effects using a simple and intuitive environment.
<img align="left" src="readMeImages/connections.png"  width="50%" style="margin-left:5px; margin-bottom:10px">



## Files
_Web Reactable_ is composed of:

- **index.html**
- **main.js**
contains the main js file, with all the functions and dependencies components

- styles.css contains the styling of the application


## Dependencies

- [**React**]: structure of the web page and of the View.
- [**Tone.js**]: a web audio framework for creating interactive music in the web intuitively.
- [**jQuery**]Library that facilitates communication between html and JS and is optimal for event handling and animation.

## Authors
Umut Fidan<br>
Roberto Leone Cicognani<br>
Claudio César Armas Monroy<br>
