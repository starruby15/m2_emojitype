### Demo 
![emojitype](https://github.com/starruby15/m2_emojitype/blob/main/images/demo.gif)

### Project Description 

For ECE 188 Project M2 EmojiType, I decided to use a gesture-recognizer through drawing numbers for the emoji keyboard.  The user draws in the canvas a digit from 1-9 
and a corresponding emoji will pop out. The list of emojis is on the side of the input area.  I felt this design would suit something like the Apple Watch so I
placed the input area in a mock-up of the Apple Watch to simulate this. 

There is also an option at the bottom to display results.  This will display the results from the model when trying to guess the digit from the drawing. The bars
on the graph represent the probability the model estimated that the drawing is the corresponding digit.  There is also the overall confidence the model guesses the
final decided digit.  Note that since this model was trained with handwritten digits, it has difficulty guessing with mouse-drawn digits. 

### Running the Model 

For the model, I recommend creating a virtual environment with python3 and running MNIST.py inside of that. 

To create the virtual environment: 
```
python3 -m venv --system-site-packages ./venv
source ./venv/bin/activate
```
Setting up and running MNIST:  
```
pip install --upgrade pip
pip install --upgrade tensorflow
pip install tensorflowjs
python MNIST.py
```

### Running the Website 

The website needs a http server in order to run.  I used brew to install http-server on my mac, but you can run http-server through npm alternatively. 

Install http-server: 
```
brew install http-server
```
Setting up and running the website:  
```
cd rootfolder 
http-server . 
```
And then open localhost:8080 in your browser. 

