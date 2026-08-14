
# Intro

Hello! I'm Peki, and in this tutorial, we're going to be covering the LMMS Compressor plugin,
what it's used for and what its various knobs and faders do.

Before we get started, it would be good to go over the basics of compression.
If you're already familiar with this part and want only to see how to use the LMMS Compressor,
feel free to skip ahead to the next timestamp shown on the YouTube timeline.

# What is Compression? What is it used for?

"Compression" is a shorthand term for "Dynamic range compression".
Most audio signals tend to have a loud and quiet part, for example:

- When playing a piano note, the loud part of the signal is at the very beginning, and the signal loudness decays over time as you hold the key down. We often refer to the loud part as the transient.
- When playing a drum loop sample, the loud parts happen at the beginning of each individual drum hit. So, each kick, snare, hat, cymbal, and so on, is a separate transient.
- When playing a riser, the volume increases over time, so the loud part happens at the very end.

A dynamic range compressor takes every transient or loud signal that is over a certain threshold and quiets it down based on how our compressor is set up.

The most common use of a dynamic range compressor is making the transients quieter, so the whole signal can become louder and more present in your mix.

# Compressors in LMMS

LMMS comes with a few compressors, most of them being provided by third party LADSPA libraries.
<!-- VIDEO TODO: add an explanation for LADSPA) -->

In our LMMS Plugins tutorials, we will always be using the plugins explicitly created by and provided by LMMS, as visible in the LMMS tab of the plugin list.
In this case, it's the plugin simply titled "Compressor".

# Compressor

Here I have a few samples and MIDI clips, all routed to a single mixer track.
Let's go ahead and place a Compressor on that track.
And I'll also add an Oscilloscope plugin so we can see the audio signal waveform and how it's being changed by the Compressor plugin.

## Useful UI Tips (Before we get started...)

<!-- TODO: This is probably gonna go into some of the other parts as a simple mention rather than its own part. -->

Before we get started with the compression aspect, I'd like to point out two useful UI tips.

1. Double tapping on the empty space above the compression parameters hides the parameters, allowing you to view the signal fully.
2. Scrolling in the empty space allows zooming in and out of the signal.

There's three curves you'll see in the empty space.

1. White: This is the actual signal
2. Gray: This is the original signal
3. Red: This is the gain reduction curve. You can combine the gain reduction curve with the dB reading on the righthand side, showing you exactly how much the signal is compressed.

## Basic parameters (Mix, In/Out Faders, In/Out Balance)

I think we've covered just about everything you need to know before we get to using the plugin.
So, let's discuss the basic parameters you'll see in almost every compressor.

## Attack, Release

First, let's cover the Attack and Release.
The two knobs allow you to specify how quickly the compression will take place.
If you set the attack to 10ms, it will take the compressor 10ms to start compressing, allowing you to keep some part of the transient intact.
If you set the release to 100ms, the compressor will continue compressing your signal down for another 100ms after the transient, unless a new transient is reached, of course!

You can find plenty of cheat sheets online for recommended attack and release values, but the LMMS Compressor features the gain reduction curve at the very top,
showing you by how much the signal has been made quieter. This lets you verify your compression is working by viewing if the transients have been properly compressed.

## Threshold, Ratio, Knee

TODO

## Auto Attack, Auto Release

## Compressor vs Inf. Ratio

## Left/Right vs Mid/Side

## RMS vs Peak Compression

## Tilt Factor

