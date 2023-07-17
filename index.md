# Rasberry Pi Document Reader for the Visually Impaired
Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:
```HTML 
<!--- This is an HTML comment in Markdown -->
<!--- Anything between these symbols will not render on the published site -->
```

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Ella S | Forest Ridge School | Computer Science | Incoming Senior


**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**
<!--
![Headstone Image](logo.svg)
  -->
# Final Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE



# Second Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/y3VAmNlER5Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone 

# First Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/CaCazFBhYKs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For my first milestone, I got my raspberry pi set up and working. I did not have a monitor to use to set up my raspberry pi, so my instructors recommended I set it up headless, meaning I set up the raspberry pi without any monitor, keyboard, or mouse. To set it up headless, I first had to install the Raspberry Pi OS (32-bit) into my Raspberry Pi’s SN Card. I had to enable SSH, Secure Shell, a service that runs on Pi that allows for secure remote connection. I then inserted the SN Card into my Raspberry Pi, connected the Pi to power and my Pi was up and running!

To connect my laptop to the Pi, I used PuTTY, a free software used for remote command-line access to Linux, which Raspberry Pi OS is. Going forward, everytime I want to connect to my Raspberry Pi, I must SSH in through PuTTY.

A challenge I faced was that my VS Code would repeatedly freeze. So, I chose to code my Raspberry Pi through a VNC Viewer, which would allow me to see the desktop of the Raspberry Pi on my laptop and then code directly on my Raspberry Pi. VNC stands  for virtual network connection.

I downloaded the RealVNCViewer and connected it to my Raspberry Pi on my local network.
At this point, I could see two programming apps on the Raspberry Pi’s desktop, which were Geany Programmer’s Editor and Thonny. I opened Thonny and ran the python command, print(“Hello World”) as a test, and it successfully printed to the terminal. 

For the last step of my first milestone, I took a test picture with the Raspberry Pi camera module. To do so, I first connected the camera to the Raspberry Pi’s camera port. Then, I ran the command on PuTTY “libcamera-still -o test.jpg” , which means I am taking a still photo and saving it on my Raspberry Pi as test.jpg. My instructor provided the picamera2 library, which I cloned onto my Raspberry Pi. I ran a couple of its files through the VNC, some that took videos and some that took different types of photos, to learn how picamera2 worked! 

To complete my project, I will need to connect all the hardware and get the code into my Raspberry Pi.


# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```

# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Raspberry Pi 4 | The raspberry pi is used to compute the words into text | $149.99 | <a href="https://www.amazon.com/CanaKit-Raspberry-Pi-Extreme-Kit/dp/B08B6F8QRV/ref=asc_df_B08B6F8QRV/?tag=hyprod-20&linkCode=df0&hvadid=563598683736&hvpos=&hvnetw=g&hvrand=12804911131851721657&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9033316&hvtargid=pla-1604885143115&psc=1"> CanaKit Raspberry Pi 4 Extreme Kit </a> |
| Mini Camera Module for Raspberry Pi | The mini camera is used to take in the words on the document as input | $9.86 | <a href="https://www.amazon.com/Arducam-Megapixels-Sensor-OV5647-Raspberry/dp/B012V1HEP4/ref=asc_df_B012V1HEP4/?tag=hyprod-20&linkCode=df0&hvadid=385286500280&hvpos=&hvnetw=g&hvrand=13998485829270770884&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9033316&hvtargid=pla-820020083673&psc=1&tag=&ref=&adgrpid=77282054583&hvpone=&hvptwo=&hvadid=385286500280&hvpos=&hvnetw=g&hvrand=13998485829270770884&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9033316&hvtargid=pla-820020083673"> Arducam 5MP Camera for Raspberry Pi </a> |
| USB Speaker for Notebook & PC | The USB Speaker will be used to play the read aloud document | $12.99 | <a href="https://www.amazon.com/HONKYOB-Speaker-Computer-Multimedia-Notebook/dp/B075M7FHM1/ref=sr_1_1_sspa?crid=28PHC6Z01OPVB&keywords=honkyob+usb+mini+speaker&qid=1688586576&s=electronics&sprefix=honkyob%2Celectronics%2C131&sr=1-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1"> HONKYOB USB Mini Speaker Computer Speaker Powered Stereo Multimedia Speaker for Notebook Laptop PC(Black) </a> |
| Momentary Button |The button is used to turn the document reader on and off | $16.99 |<a href="https://www.amazon.com/BOJACK-Electronics-Potentiometer-tie-Points-Breadboard/dp/B099MQV8ZW"> Bojack Electronics Fun Kit <a>|
| LED Light | The LED light shows whether the document reader is on or off -- comes in the same kit as the button |$16.99 |<a href="https://www.amazon.com/BOJACK-Electronics-Potentiometer-tie-Points-Breadboard/dp/B099MQV8ZW"> Bojack Electronics Fun Kit <a>|

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
