# Sonic Pi Live - Change the Code Task

##Step 1: Do you have a GitHub account?

Make sure that you have signed up for [GitHub here](https://github.com/). 

##Step 2: Make a copy of this **repository**

A repository is a type of folder on github. Making a copy of a respoistory is called **forking**. Click on the 'Fork' button at the top of the screen on the right hand side, and a copy of everything in this respoitory called *change-caode-task* will appear in your account.

![](forking.png)

##Step 3: Locate the code!


Now navigate back to your account and find the starter code called . The code will look like this but will be in a text file called `code.rb`:

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


