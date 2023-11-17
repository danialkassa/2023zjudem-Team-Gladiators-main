  <h1 style="font-size:2vw"><span style="color:black">Introduction to Arduino</span></h1>
Arduino is a prototyping platform (open source) based on easy-to-use hardware and software. It consists of a programmable circuit board called a microcontroller and off-the-shelf software called the Arduino IDE (Integrated Development Environment) for writing and uploading computer code to the physical board.
<h1 style="font-size:1.5vw"><span style="color:black">The main features are:</span></h1>
The Arduino board is able to read analog or digital input signals from different sensors and convert them into outputs such as activating motors, turning on/off LEDs, connecting to the cloud and many other operations.

You can control board functions by sending a set of instructions to the microcontroller on the board through the Arduino IDE (upload software for short).

Unlike most previous programmable circuit boards, Arduino does not require additional hardware (called a programmer) to load new code onto the board. You just use a USB cable.

Additionally, the Arduino IDE uses a simplified version of C++, making it easier to learn programming.

Finally, Arduino offers a standard form factor that breaks the functionality of a microcontroller into easier-to-use packages
<h1 style="font-size:1vw"><span style="color:black">Types of Arduino boards</span></h1>

Various Arduino boards are available, depending on the microcontroller used. However, all Arduino boards have one thing in common: they are programmed through the Arduino IDE.

The differences are based on the number of inputs and outputs (number of sensors, LEDs, and buttons that can be used on a single board), speed, operating voltage, form factor, etc. Some boards are designed to be embedded and do not have a programming interface (hardware), so you will need to purchase them separately. Some can run directly from a 3.7V battery; others require at least 5V.

Below is a list of the different Arduino boards available.
<h1 style="font-size:1vw"><span style="color:black">Some Boards are</span></h1>

<link rel="stylesheet" href="css/bootstrap-grid.min.css"/>
<div class="demo">
        <div class="container">
            <div class="row text-center">
                <h1 class="white"></h1>
            </div>

<div class="row">
                <div class="col-md-4 col-sm-6">
                    <div class="arduino">
                        <div class="pic">
                            <img src="image/ar3.jpg">
                            <ul class="social">
                                <li><a href="https://store.arduino.cc/products/arduino-uno-rev3" class="fab fa-facebook">Arduino UNO R3</a></li>
                            </ul>
                        </div>
                        <div class="team-content">
                            <h3 class="title"></h3>
                            <h3><a href="https://store.arduino.cc/products/arduino-uno-rev3" class="title"></a></h3>
                        </div>
                    </div>
                </div>

<div class="col-md-4 col-sm-6">
                    <div class="arduino">
                        <div class="pic">
                            <img src="image/ar4.jpg">
                            <ul class="social">
                                <li><a href="https://store.arduino.cc/products/arduino-mega-2560-rev3" class="fab fa-facebook">Arduino Mega 2560 Rev3</a></li>
                            </ul>
                        </div>
                    </div>
                </div>

<div class="col-md-4 col-sm-6">
                    <div class="arduino">
                        <div class="pic">
                            <img src="image/ar5.jpg">
                            <ul class="social">
                                <li><a href="https://store.arduino.cc/products/arduino-leonardo-with-headers" class="fab fa-facebook">Arduino Leonardo</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            


<div class="col-md-4 col-sm-6">
                    <div class="arduino">
                        <div class="pic">
                            <img src="image/ar6.jpg">
                            <ul class="social">
                                <li><a href="https://store.arduino.cc/products/arduino-uno-wifi-rev2" class="fab fa-facebook">Arduino UNO WiFi Rev2</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>

<br><h1 style="font-size:1.5vw"><span style="color:black">Arduino Installation</span></h1>

Here is a simple steps how to set up the Arduino IDE on our computer and prepare the board to receive the program via USB cable.

<br><h1 style="font-size:1.5vw"><span style="color:black">Step 1 </span></h1>
 First, you must have Arduino board (you can choose the one you like) and a USB cable. If you use an Arduino UNO, Arduino Duemilanove, Nano, Arduino Mega 2560 or De="coliecimila, you will need a standard USB cable (A plug to B plug). The picture below shows the type of USB printer you will connect to.
 <br><div class="loader"><img src="image/ar.jpg" alt="#" /></div>

<br><h1 style="font-size:1vw"><span stylor:black">Step 2 - Download the Arduino IDE software.</span></h1>

Click here to [download](https://support.arduino.cc/hc/en-us/articles/360019833020-Download-and-install-Arduino-IDE),  After the file download is complete, unzip the file.
                                                                                         <br>
<br><h1 style="font-size:1vw"><span style="color:black">Step 3 - Power on the board.</span></h1>
<br>The Arduino Uno, Mega, Duemilanove and Arduino Nano draw power automatically via USB connection to a computer or external power source. If you use an Arduino Diecimila, you must ensure that the board is configured to draw power from the USB connection. Power selection uses a jumper, a small piece of plastic that fits two of the three pins between the USB and power jacks. Check that it's on the two pins closest to the USB port. Connect the Arduino board to the computer using a USB cable. The green power LED etc. (labeled PWR) should glow.
<br><h1 style="font-size:1vw"><span style="color:black">Step 4 - Start Arduino IDE.</span></h1>
<br>After downloading the Arduino IDE software, you need to unzip the folder. In the folder you can find the application icon with the infinity label (application.exe). Double-click the icon to launch the IDE.

<br><div class="loader"><img src="image/ar1.jpg" alt="#" /></div>
<br>
<br><h1 style="font-size:1vw"><span style="color:black">Step 5 - Open your first project.</span></h1>
Once the software starts, you have two options:

  Create a new project.
  Open an existing project example.
To create a new project, select Flie→New.
<br><div class="loader"><img src="image/ar2.jpg" alt="#" /></div>
<br>
<br><h1 style="font-size:1vw"><span style="color:black">Step 6 - Choose your Arduino board.</span></h1>
<br>In order to avoid any errors when uploading the program to the board, it is necessary to choose the correct Arduino board name that matches the board connected to the computer.

Go to Tools → Board and select your board.
<br> After selecting the right board, then select the serial device for the Arduino board. Go to Tools→Serial Port menu. This is probably COM3 or higher (COM1 and COM2 are usually reserved as hardware serial ports). To figure it out, you can disconnect your Arduino board and reopen the menu, then the disappearing entry should be the Arduino board. Reconnect the board and select that serial port. Then Upload - Simulate.
<br>
<br>For detail Explanation: [Click Here](https://www.w3cschool.cn/arduino/arduino_overview.html)

For a set of example programs of Input and Output: [Click Here](https://www.nexmaker.com/doc/5arduino/Arduino_Input.html) or [Here](https://www.nexmaker.com/doc/5arduino/Arduino_output.html) respectively.
