## Tags

### v0.1

**The first happy/sad face assignment has to do with displaying two faces forever. The two faces will appear on the led screen on 5000ms intervals. 
* JS file: basic.forever(function () {
    basic.showIcon(IconNames.Happy)
    basic.pause(5000)
    basic.showIcon(IconNames.Sad)
    basic.pause(5000)
})**

### v0.2

**This assignment took the previous coding and gave it inputs. Instead of the faces appearing forever, the micro bit now displys them after either button "A" or "B" is pressed.
* JS file: input.onButtonPressed(Button.A, function () {
    basic.showLeds(`
        . # . # .
        . . . . .
        # . . . #
        . # # # .
        . . . . .
        `)
})
input.onButtonPressed(Button.B, function () {
    basic.showLeds(`
        . # . # .
        . . . . .
        . # # # .
        # . . . #
        . . . . .
        `)
})
basic.clearScreen()**


# Cello-Tuner-Metronome

#### Goal

**Music is a passion of mine, therefore, I decided to turn my Micro Bit into a cello tuner and metronome.**

#### Design process

**I chose a cello for the instrument because it is what I know how to play. It is cello specific because the tones played and displayed are A, D, G, C; the open strings on a cello from high to low. I contemplated for a while on what inputs I wanted to cause the tone for each note. Did I want one button to play all four? Or have buttons A and B play two each? I ended up settling with four seperate inputs for each note, because it was easiest to repeat one note if that string was severely out of tune on the cello. I also struggled with getting the letter to display on the led's while the tone was playing, instead of the tone playing and then the led disply or vise versa. I solved this issue with the "basic.clearscreen" command placement. I originally had it after the led display which caused the issue. I noticed when I was looking on the microbit website and other resources that coding microbits to be tuners is common compared to other ideas. So I wanted to take it one step further and make it a metronome using bpm command option. I wanted to give myself some variety and allow for 120 bpm, which is the lower end bpm standard for most Allegro peices of music, and 72 bpm, which is the most common bpm for an Arpegio peice. Finally, in order to hear all the tones, an external speaker will need to be connected. I can do so by connecting allegator wires to the "GND" and "0" terminals on the micro bit to a speaker or pair of headphones.**

#### JS Constructs & objects

**This project includes some basic commands such as, "showled," "shownumber," "clearscreen," "onstart," and "showstring." It heavily relied on using the microbit inputs that are included in the device like the buttons, tilt, and facing options. I also used "playtone" commands to program the tuner portion. To set the metronome bpms I used the "setTempo" commands under the same category. I wanted to implement loops into the project too so I coupled that with the play tones to hear the note longer and save the user from having to perform the inputs over and over again.**


