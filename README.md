# Sonic Pi Live - Change the Code Task

##Step 1: Do you have a GitHub account?

Make sure that you have signed up for [GitHub here](https://github.com/). This [github cheat sheet may come in handy](https://education.github.com/git-cheat-sheet-education.pdf) too.

##Step 2: Make a copy of this **repository**

A repository is a type of folder on github. Making a copy of a respoistory is called **forking**. Click on the 'Fork' button at the top of the screen on the right hand side, and a copy of everything in this respoitory called *change-code-task* will appear in your account.

![](forking.png)

##Step 3: Locate the code!

Now navigate back to your account and find the starter code called *code.rb*. The code will look like this but will be in a text file:

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

Next you will want to transfer the text file containing the code from your computer to your Raspberry Pi. You can use the *copy to clipboard* button to copy and paste the code into a text file on your computer, or you can download the entire repository using the *download zip* button. Once you have file containing the code, transfer it to a Raspberry Pi using a removable storage device such as a usb memory stick.

##Step 5: Change the code

Open the text file on your Raspberry Pi and copy and paste the code into Sonic-Pi. Change this code to make it more interesting in any way that you like. It is now your version of *code.rb*. When you have finished your code, copy and paste it back into a text file and save it onto the usb memory stick.

##Step 6: Upload the changed code to Github

The easiest way for you to do this without having to use the command line is to open the file on github by clicking on the *code.rb* file in your forked repository. (Not our original!) Then click on *edit*. You can then paste your new code over the top. To save your code you need to **commit** it to the repository. You will notice that there is a comment box in which you can give a description to the code that you have changed. Add an explanantion here and then click on *ommit Changes**.

![](commit.png)

##Step 7: Share and Comment

Follow [Sam](http://github.com/samaaron) or [Carrie Anne](http://github.com/missphilbin) and anyone else from the project. Then you will be able to see their forked repositories and their changed versions of code.rb

You can comment on their work by..

##Step 8: Learn more about GitHub in Education

You can learn more about how to use [GitHub in Educcation here](https://education.github.com/guide). Including steps on administrating accounts for students. 



