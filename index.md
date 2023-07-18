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

My third milestone was recreating my LED and button circuits using alligator clips and refiguring the command line commands in the document reader code into PiCamera2 function calls. 
Initially, I used a breadboard, inside my cardboard box, to connect my LED and button to the raspberry pi. So, every time I ran my document reader, I had to open the box to press the button. Instead, I wanted my button and LED to poke out through the top of my cardboard box, so that users would be able to easily press the button and see the LED flash on and off. 
When connected to the breadboard, my button was way shorter than my LED light. If I had my breadboard right under the cardboard box, I would not be able to have the LED and button poking out at the same height, and the resistor and wires would also have to stick out. So, I wanted to figure out a way to get my LED and button off the breadboard. 
My instructor recommended I solder the wires together, but I didn’t have an outdoor space to work and didn’t want to breathe in the fumes inside. So, I ultimately decided to use alligator clips to put the circuit together. First, I made some cuts in a piece of cardboard, in which I stuck the button and LED at different heights – with the button sitting on top and the LED hanging slightly below. Then, I cut a hole out of my cardboard box and placed my piece of cardboard above it. Within my box, I clipped one of the ends of the alligator clips to the dupont wires that connected to the Raspberry Pi and the other ends to the wires of the LED and button. Although the wires and alligator clips look slightly messy inside the box, they worked! 
The second part of my first milestone was making my document reader more discreet and functional by allowing the stand to fold down, adding hinges to the cardboard box, and creating a cardboard extender so my document reader can hold longer documents.
I followed a Youtube tutorial on how to create hinges out of cardboard and paper, which worked pretty well! I then hot-glued them onto my box. 
Using my prior knowledge and the cardboard hinge tutorial, I devised a solution that would allow my camera stand to be foldable but also hold up and stand straight once unfolded. This is what I came up with:
To create the cardboard extender, I cut out a strip on the side of my box and inserted a piece of cardboard almost as wide as the box. For the extender to not run into my wires, I cut out the inside, leaving the extender as a frame. 




# Second Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/y3VAmNlER5Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

My second milestone was setting up hardware and importing the document-reader code. 
In the tutorial, the base of the document reader is an 8x8 wooden box, which holds the Raspberry Pi and speaker and acts as a surface for the documents to lie on. I used cardboard instead, as I had a bunch of boxes at home. I cut two squares out of cardboard out of a box and bent down the edges to create a new, smaller, 8x8 box. Then, I added a hole to the bottom half for my Raspberry Pi’s power cable to go into. 
I added holes to the top of the cardboard box that looked like a speaker grill, placed the speaker below the holes, and connected the speaker to my Raspberry Pi. I also cut a strip in my cardboard box for my camera cable to go through, allowing my camera to be outside the box while the raspberry pi is inside the box. 
Using the command “git clone https://github.com/rgrokett/PiTextReader.git” on puTTY, I cloned the PiTextReader code folder from the instructions into my RaspberryPi. The code takes a picture of an item, converts it to plain text using Tesseract OCR (Optical Character Recognition), an external engine, and then speaks the text using text-to-speech. When I ran the code, I heard the expected “Ok ready” and “Ok working,” but did not hear any text read aloud. 
After testing the camera by taking a few stills, I realized that my text was too small for the camera to pick up. I tried adjusting the camera height and some of the libcamera properties, including sharpness and picture dimensions, but no small words remained illegible. So, I decided to instead use a document with larger, bolder text–it worked!


# First Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/FdgOZ_EXeZc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

Hi, my name is Ella and I’m a rising senior at Forest Ridge School of the Sacred Heart. My project is the Easy-To-Use document reader. The document reader can be used by those visually impaired, or by anyone who wants a document read out loud. The document reader consists of a camera, which takes in the words, and a speaker, which projects the speech.
For my first milestone, I got my raspberry pi set up and working. I did not have a monitor to use to set up my raspberry pi, so my instructors recommended I set it up headless, meaning I set up the raspberry pi without any monitor, keyboard, or mouse. To set it up headless, I first had to install the Raspberry Pi OS (32-bit) into my Raspberry Pi’s SN Card. I had to enable SSH, Secure Shell, a service that runs on Pi that allows for secure remote connection. I then inserted the SN Card into my Raspberry Pi, connected the Pi to power and my Pi was up and running!
To connect my laptop to the Pi, I used PuTTY, a free software used for remote command-line access to Linux, which Raspberry Pi OS is. Going forward, every time I want to connect to my Raspberry Pi, I must SSH in through PuTTY.
A challenge I faced was that my VS Code would repeatedly freeze. So, I chose to code my Raspberry Pi through a VNC Viewer, which would allow me to see the desktop of the Raspberry Pi on my laptop and then code directly on my Raspberry Pi. VNC stands for virtual network connection.
I downloaded the RealVNCViewer and connected it to my Raspberry Pi on my local network.
At this point, I could see two programming apps on the Raspberry Pi’s desktop, which were Geany Programmer’s Editor and Thonny. I opened Thonny and ran the Python command, print(“Hello World”) as a test, and it successfully printed to the terminal. 
For the last step of my first milestone, I took a test picture with the Raspberry Pi camera module. To do so, I first connected the camera to the Raspberry Pi’s camera port. Then, I ran the command on PuTTY “libcamera-still -o test.jpg”, which means I am taking a still photo and saving it on my Raspberry Pi as test.jpg. My instructor provided the picamera2 library, which I cloned onto my Raspberry Pi. I ran a couple of its files through the VNC, some that took videos and some that took different types of photos, to learn how picamera2 worked! 
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
