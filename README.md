# Stepify [![Build Status](https://travis-ci.org/rishab2113/Stepify.svg?branch=master)](https://travis-ci.org/rishab2113/Stepify)

# Inspiration
Generally, the elderly and visually impaired people walk with someone by their side. But what if nobody is around to help? We were very concerned about the fact that help may not be always available so we wanted to make a positive impact on the elderly and visually impaired people. Nowadays, the elderly want to have independence and not always want people around to monitor them, so we also catered to their independence.   

# What does Stepify do?
Our web-app takes input in the form of images through the raspberry pi camera, processes them and through the ultrasonic sensor, it gives accurate distance calculation between an object and the person with the camera. Also, if the distance from the object to the person is small, a warning signal is sent out to the person in the form of speech through their speaker or headset. If the person does not respond to this message within 1 minute, an emergency call is sent out to 911 and another emergency contact of the user's choice (registered in the firebase database).

# How did we build it?
We started off with setting up the Raspberry Pi 3 and it's method of input. We used multiple Python scripts to get input from the pi camera, the ultrasonic sensors and accelerometers. The data from the camera was passed through the Clarifai API which generates tags based on the image after it has been processed. We used Python to refine the results that we received from the API. The inputs from the ultrasonic sensors and accelerometers are processed using our Python script, and the results are calculated and returned to the user on the Web-App. We integrated all the components to get a web-app and a device to go along with it.

# What were the challeneges we ran into?
Our Raspberry Pi 2 was not compatible with the accelerometer so we had to figure out a way to get it working. The code for sending images to the Clarifai server took us a while to figure out, but we managed to complete the task. Coding the accelerometer and ultrasonic sensor was a challenge as we had not done something like this before.

# Accomplishments that we're proud of!
Firstly, we are extremely proud of this prototype of our product. Secondly we got past all challenges of the project as a team and helped each other out whenever necessary.

# What did we learn from this experience?
We learned how to use a Raspberry Pi in depth and its functions. We learned how to use and implement the Clarifai, Adafruit and Twillio API's respectively. Most importantly, my team learned better teamwork and cooperation among each other.

# Next stages of this project...
Our passion for helping the elderly and visually impaired will always exist, and we will continue to take this project on further in order to make it a successful product and make a change in society foe a greater good.



## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```
