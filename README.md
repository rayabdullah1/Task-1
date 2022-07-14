# Task-1
### Speech to text &amp; ESP32 steps in Arduino

## (1) Speech to text
Create a web page that converts the Audible sound into text, either in Arabic language, by using JavaScript, CSS, or HTML.

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
