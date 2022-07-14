# Task-1
### Speech to text &amp; ESP32 steps in Arduino

## (1) Speech to text
**Create a web page that converts the Audible sound into text, either in Arabic language, by using JavaScript, CSS, or HTML.**


![‏‏لقطة الشاشة (124)](https://user-images.githubusercontent.com/108306624/178945560-e5f06fe7-a8f0-4403-aa19-4caa872e35ee.png)
**-Receive the oudio in Arabic and then wrote it.**

![‏‏لقطة الشاشة (125)](https://user-images.githubusercontent.com/108306624/178945572-da3d27f0-5929-466f-a884-188842fdeaa5.png)
**-Also, a pause recording button has been added.**

**HTML** code:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Speech to text</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css">
</head>
<body background="image1.jpg">
    <div class="container">
        <h1 class="text-center mt-5">
            speech to text in Arabic language
        </h1>
            <div class="form-group">
                <textarea id="textbox"  rows="6" class="form-control"></textarea>
            </div>
            <div class="form-group">
                <button id="start-btn" class="btn btn-danger btn-block" style="background-color:black ;">
                    Start Recognition
                </button>
                <button id="pause-record-btn" class="btn btn-danger btn-block" style="background-color:black;">
                    Pause Recognition
                </button>
                <p id="instructions"> 
                        Press the Start button </p>
            </div>
    </div>

</body>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
<script src="script.js"></script>
</html>
```

## (2) ESP32 steps in Arduino
**Writing the steps that describe how this piece works.**

#### Steps:
1. Download Arduino IDE 1.8.19 on your device.
2. Go to Tools > Board >  Boards Manager > in search bar write "esp32" > click on install.
3. !!If ESP32 didn't show then go to File > Preferences > putting link of the library. 
4. Go to Tools > Board >  ESP32 Arduino > WEMOS D1 MINI ESP32.
5. Go to Tools > Port and select a COM port available.
6. !!if the port not available, you have to check the update drivrs from device manager.
7. go to File > Examples > Basics > Blink. To make sure the piece is working and programmed correctly

code:
```
/*
  Blink

  Turns an LED on for one second, then off for one second, repeatedly.

  Most Arduinos have an on-board LED you can control. On the UNO, MEGA and ZERO
  it is attached to digital pin 13, on MKR1000 on pin 6. LED_BUILTIN is set to
  the correct LED pin independent of which board is used.
  If you want to know what pin the on-board LED is connected to on your Arduino
  model, check the Technical Specs of your board at:
  https://www.arduino.cc/en/Main/Products

  modified 8 May 2014
  by Scott Fitzgerald
  modified 2 Sep 2016
  by Arturo Guadalupi
  modified 8 Sep 2016
  by Colby Newman

  This example code is in the public domain.

  https://www.arduino.cc/en/Tutorial/BuiltInExamples/Blink
*/

// the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(1000);                       // wait for a second
}
```

### If you want to try it. [ESP32 simulator](https://wokwi.com/projects/new/esp32)
