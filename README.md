# Sonic Pi Live - Change the Code Task

##Step 1: Do you have a GitHub account?

Make sure that you have signed up for [GitHub here](https://github.com/). 

##Step 2: Make a copy of this **repository**

A repository is a type of folder on github. Making a copy of a respoistory is called **forking**. Click on the 'Fork' button at the top of the screen on the right hand side, and a copy of everything in this respoitory called *change-caode-task* will appear in your account.

![](forking.png)

##Step 3: Locate the code!

Now navigate back to your account and find the starter code called `code.rb`. The code will look like this but will be in a text file:

````ruby
define :drums do
  sample :drum_heavy_kick, rate: 0.75
  sleep 0.5
  sample :drum_heavy_kick
  sleep 0.5
end

define :synths do
  use_synth :mod_pulse
  use_synth_defaults amp: 1, mod_range: 15, attack: 0.03, release: 0.6, cutoff: 80, pulse_width: 0.2, mod_rate: 4
  play 30
  sleep 0.25
  play 38
  sleep 0.25
end

in_thread(:drums){loop{drums}}
in_thread(:synths){loop{synths}}
````

##Step 4: Copy the code to your Raspberry Pi

Next you will want to transfer the text file containing the code from your computer to your Raspberry Pi. Click on the button labelled *raw* and save the file onto a removable storage device like a USB memory stick. Once the file has completed the download, remove it safely from the computer and plug it into your Pi. Copy the file from the usb drive to a folder on the Pi. 

##Step 5: Chnage the code

Open the text file on your Raspberry Pi and copy and paste the code into Sonic-Pi. Change this code to make it more interesting in any way that you like. It is now your version of *code.rb*. When you have finished your code, copy and paste it back into a text file and save it onto the usb memory stick.

##Step 6: Upload the changed code to Github



##Step 7: Learn more about GitHub in Education

You can learn more about how to use [GitHub in Educcation here](https://education.github.com/guide). Including steps on administrating accounts for students. 



