SYMED-the Health Assistant

App Description:

Symed is a personal health care application that uses the cartoon Baymax from the Big Hero 6 as a virtual personal assistant. It asks the user about the emotion that currently precedes over them and tells them how to control the emotion. It acts as a virtual buddy and is also designed to act as a general physician that helps to cure simple symptoms such as cold, fever, cough, headache among few others. 

Prerequisites:

One would require Basic Python Programming knowledge along with familiarity on using the PYSimpleGUI module. One must also require a basic knowledge in JavaScript and HTML

Requirements:

	The computer should have Python 3.7 or above installed.
	The following modules should be downloaded through the command prompt:
	The module PySimpleGUI should be downloaded using the code: pip install PySimpleGUI
	The module playsound should be downloaded using the code: pip install playsound

Learning Outcomes:

	 Learnt how to use radio buttons on the PySimpleGUI
	Learnt to use the webbrowser module to launch an internet website.
	Learnt to animate Gif’s using sg. Image in PySimpleGUI
	Learnt how to call a python file inside a python file, use it as a function to implement it on demand, using exec(open()) command.
	Used HTML pages for storing content, JavaScript and CSS for making audio
	Learnt to make quiz application that checks the user’s answers and prints out the scores in the end.
	Learnt the file.write() function that writes the code in another text file. Even the datetime.date.now which gives the current date and for time X.strftime was used.
Modules, Function & Parameters:

1.	 PySimpleGUI-
•	theme- it is used to add customized color as background for all the windows. It has been set as Material1 which gives a sky-blue color.
•	Image-It is used to add images into the window.
o	Key- It is used as a uniquely identifiable character that is used to search the following element.
o	Size- it is used to specify the size of the image in pixels
o	Tooltip-it has been used to type introductory message for the user.
•	 Window-It is used to create the window
o	Read-it is used to read the code for the window and run it. The parameter timeout has been added to help in the updating the window for equal intervals of time.
o	FindElement- it is used to specifically find the element in the code using its uniquely identifiable key.
o	UpdateAnimation-it is used to update the window and give the animation. The speed of the animation can be controlled using the parameter time_between_frames
o	Finalize- this is used to call out a second window in case of an on click event.
•	Text- it is used to present text to the users in the window.
•	Radio buttons-
o	Key- It is used as a uniquely identifiable character that is used to search the following element.
o	Enable events- it is used to enable events that can be linked with other codes to enable continuity in the code. It accepts only Boolean values
•	Buttons-
o	Key- It is used as a uniquely identifiable character that is used to search the following element.
o	Enable events- it is used to enable events that can be linked with other codes to enable continuity in the code. It accepts only Boolean values
o	Button color- it is used to change the button color from one to another. It needs two have two parameters in order to work properly one is the color that is currently in the button and the other is the color you want in the button.
2.	Playsound-It is used to play audio files of .mp3 and .wav files. it has only one parameter. The file path needs to entered in order to play the audio.
3.	Webbrowser- it is used to open a website using URL in python.
•	New- it is a parameter used to decide if the website will open in the same browser or will take a different browser on every click event. The new has been set to new=2 i.e., it will take different browser on every on click event. If this is not needed, simply go with new=0.
•	Open-it is used to run and open the URL code. It takes two parameters. One is the URL and the other is new.

Q &A:

1.	What are the problems faced while coding the front end/back end and any specific codes to avoid/use while improvising the code?

The problems that were faced while coding the front end/back end is as follows:
•	Was unable to animate the GIF using popup. Animated as the it would lead to a high CPU usage for GIF of larger size and would thus slow down the computer. Solution- Use sg. Image to show the GIF and animate using UpdateAnimation. 
•	Was not able to pause or stop the audio on click. Solution- You could use pypat module instead of playsound module.
•	Error due to the exit button that said “You are trying to open a closed file”. Solution-Set a flag element to true where the window.read() is done, initially then changed it to false when the exit button is pressed.
•	Name is not defined error (because we called a function before declaration). Solution- First define a function, before calling it.


References:

1.	 Cookbook-PySimpleGUI
Link-https://pysimplegui.readthedocs.io/en/latest/cookbook/


2.	 Animate GIF-Stack Overflow
Link-https://stackoverflow.com/questions/61802250/pysimplegui-animate-a-gif-in-window


3.	Playsound – RealPython1
Link-https://realpython.com/playing-and-recording-sound-python/#:~:text=Playing%20Audio%20Files,-Below%2C%20you'll&text=python%2Dsounddevice%20and%20pyaudio%20provide,a%20few%20lines%20of%20code.


4.	 Playsound installation guide – PyPI
Link-https://pypi.org/project/playsound/


