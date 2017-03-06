# Xcode Breakpoint Sounds

![Sounds](/xcode_debug_sounds.png?raw=true "Sounds")

**Xcode Breakpoint Sounds** is a custom collection of audio files specifically made for use with Xcode's _Sound_ breakpoint action.

For more info, see the [complete blog post](http://sound-of-silence.com/?article=20170306) on these sounds.

## :speaker: Why use sounds?

The biggest downside of typical breakpoints is that they freeze everything in its tracks and forcibly remove you from the context of the app you're debugging. Sometimes you'll want to gain a better understanding of how and when certain code is executing as you use the app in a fluid, natural manner.

**Audible breakpoints** have several unique advantages. They allow you to:

- Use the app you're debugging in a natural, fluid manner, without interruptions
- Keep your eyes completely focused on the UI or visual behaviors of that app
- Obtain immediate feedback when reproducing timing-sensitive bugs, since the app does not need to be paused for the breakpoints to communicate the intended information
- On macOS, avoid unwanted side effects caused by the app being deactivated when Xcode is brought forward (this is especially useful when debugging issues with popovers or utility panels, etc.)

## What makes a 'good' breakpoint sound?

You'll quickly notice that Xcode's default sounds are fairly limited. Breakpoint sounds should ideally meet several criteria:

- The audio files should be small in size (fast to load, quick to initiate playback)
- They should be short in duration, to avoid long pauses while the breakpoint sound action is run
- They should be uniquely discernible from each other, in cases where multiple sounds might play close together
- Each playback should be distinct (so that the number of times the breakpoint sound is played is clear)
- They should ideally convey some kind of meaning, or improve the context of debugging in some way

This collection attempts to provide a well-rounded, multi-purpose set of debugging sounds which meet all of the above criteria.

## How to use

:large_orange_diamond: **Option 1: Adding to Xcode**

The easiest way to use these sounds is to add them to Xcode's breakpoint editor sound menu:

1. Download the sounds
2. Copy the audio files to `~/Library/Sounds`
3. Quit and relaunch Xcode

:large_orange_diamond: **Option 2: Using AFPlay**

If you don't wish to modify your `~/Library/Sounds` folder, you can also easily play these sounds by using the _Shell Command_ breakpoint action, rather than the _Sound_ action.

Simply create a breakpoint which calls the `afplay` command and provide the file path to the sound effect you want to play as the argument. With this approach, you can make use of any arbitrary audio file in any location.

## The Sounds


While these may not be amazing audio effects from a creativity or production-value standpoint, I believe they are particularly good choices for debugging. The example context listed for each audio file is obviously just a suggestion - they can be used however you like. The idea is simply to choose an effect which has some subjective association which makes it easier to recognize each breakpoint, particularly when using multiple breakpoints together. 

| Sound | Example Context |
| --- | --- |
| Xcode_Collect | Adding object to a collection (sound is similar to collecting an item or increasing your score in a video game) |
| Xcode_Pop | Removing an item from a collection (e.g. 'popping' an object from a stack), freeing memory or releasing an object |
| Xcode_Bzzt | Error or unexpected condition, useful for breakpoints in code that should not be hit |
| Xcode_Swish | Releasing objects, freeing memory, exiting methods/functions, early returns |
| Xcode_Click | Marker or tick sound (especially short, useful for breakpoints which may occur in rapid succession) |
| Xcode_Error | Error or unexpected conditional |
| Xcode_Knock | File writes, counter increment or decrement, etc. |
| Xcode_Punch | Costly operation or code which is performing significant work |
| Xcode_Zip | General purpose |
| Xcode_Quack | General purpose |
| Xcode_Bird | General purpose |
| Xcode_Chime | General purpose |

## Author

**Matt Reagan** - Website: [http://sound-of-silence.com/](http://sound-of-silence.com/) - Twitter: [@hmblebee](https://twitter.com/hmblebee)

## Licensing / Credits

These sound effects were selected from a library of royalty-free audio files, which I've amassed over the years for use with some of my [game development projects](http://sound-of-silence.com/?page=gamedev). No copyrights or author credits are known to me; each audio file here is believed to be in the public domain. If you have questions on the source of any of these audio files please feel free to contact me.

