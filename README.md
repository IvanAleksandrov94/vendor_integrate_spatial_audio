# Integrate spatial audio

## Spatial audio and head tracking

 Android 13 introduces a standard way for OEMs to support spatial audio and head tracking without the need for vendor-specific customizations or SDKs.

Spatial audio is a technology used to create a sound field surrounding the listener. Spatial audio enables users to perceive channels and individual sounds in positions that differ from the physical positions of the transducers of the audio device used for playback. For instance, spatial audio offers the user the ability to listen to a multichannel soundtrack over headphones. Using spatial audio, headphone users can perceive dialogue in front of them, and surround effects behind them, despite having only two transducers for playback.

Head tracking helps the user understand the nature of the spatialized sound stage being simulated around their head. This experience is effective only when the latency is low, where latency is measured as the time between when the user moves their head and the time they hear the virtual speaker position moving accordingly.

Android 13 optimizes for spatial audio and head tracking by offering spatial audio processing at the lowest possible level in the audio pipeline to obtain the lowest possible latency.

# Architecture

The modified Android audio framework and API in Android 13 facilitates the adoption of spatial audio technology across the ecosystem.

The following figure illustrates the spatial audio related changes made to the audio pipeline architecture with Android 13:

[<img src="/source/spatial-audio.png"/>]
[<img src="/source/spatial-sys-arch.png"/>]