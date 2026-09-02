
# Intro

Hello! I'm Peki, and in this tutorial, we're going to be covering the LMMS Compressor plugin,
what it's used for and what its various knobs and faders do.

Before we get started, it would be good to go over the basics of compression.
If you're already familiar with this part and want only to see how to use the LMMS Compressor,
feel free to skip ahead to the next timestamp shown in the video's description.

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

# Setup

Here I have a few samples and MIDI clips, all routed to a single mixer track.
Let's go ahead and place a Compressor on that track.
And I'll also add an Oscilloscope plugin so we can see the audio signal waveform and how it's being changed by the Compressor plugin.

# Useful UI Tips (Before we get started...)

Before we get started with the compression aspect, I'd like to point out two useful UI tips.

1. Double tapping on the empty space above the compression parameters toggles hiding the parameters, allowing you to view the signal fully.
2. Scrolling in the empty space allows settings the decibel range of the signal display.

There's four curves you'll see in the empty space.

1. White, which is the output signal
2. Gray, which is the input signal
3. Red, which is the gain reduction curve
4. Green, which is the compression curve

You can combine the gain reduction curve with the dB reading on the righthand side, showing you exactly how much the signal is compressed.

# Parameters

I think we've covered just about everything you need to know before we get to using the plugin.
So, let's discuss the parameters of the plugin.

## Mix, In/Out Faders

Mix allows setting the balance between the dry, original signal and the wet, compressed signal.

In and Out faders allow changing the volume of the input and output signal.

## Threshold

Threshold defines the signal level where the compressor starts taking place.
It is measured in decibels and appears in the UI as a dotted green horizontal line.

Any signal below the threshold will pass through unaffected.
Once a signal crosses above the threshold, the compressor begins applying gain reduction to control the volume.

## Ratio

Ratio controlls how far the compressor must turn the volume of a signal down after it crosses the threshold.

It's called the ratio beacuse the value we set is the exact ratio of the compression.
For example, a 4:1 ratio means that for every 4 dB the input signal rises above the threshold, the output signal only increases by 1 dB.

Lower ratios offer gentle control, while higher ratios compress the signal more.

## Attack, Release

Attack controls how quickly the compressor ramps up its gain reduction when a transient or loud signal hits.
For example, if you set a slower attack time, the compressor reacts more gradually.
This is often used to allow the initial part of a transient to pass through untouched before clamping down.
And if you set a shorter attack time, the compressor will react faster, compressing more of the signal.

Release controls how quickly the compressor eases up on the gain reduction,
allowing the signal to return to its normal level after a transient passes.

## Knee

Knee allows smoothing out the compression curve, and shapes how the compressor transitions into action as the signal crosses the threshold.

Lower values create what is called a hard knee.
A hard knee makes the compressor clamp down immediately the exact moment the signal crosses the threshold, which can sound more aggressive or punchy.

Higher values smooth out the curve and create a soft knee.
A soft knee gradually introduces compression as the signal approaches and crosses the threshold, creating a smoother, more transparent, and natural-sounding transition.

---

The following parameters are less commonly seen in compressors, but are nevertheless very useful.

## Left/Right vs Mid/Side, In/Out Balance

The LMMS Compressor allows biasing the input stereo signal.
Biasing two signals refers to giving more presence to one than the other.
Most often, this involves changing the volume of the left and right signals (also known as panning),
or chaning the volume of the mid and side signals.
Those are the two bias modes in the LMMS Compressor, and biasing the input and output signals is done with the Balance knobs.

- LEFT/RIGHT is used for signal panning, and is the default. Left is left and right is right.
- MID/SIDE is used for biasing the mid/side signal. Left is mid and right is side.

## Auto Attack, Auto Release

## Compressor vs Inf. Ratio

## RMS vs Peak Compression

## Tilt Factor

