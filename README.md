# antiradio
This is a simulator for an audio art project. 

##Design Goals

Radios convert signals to sound differently from how computers convert files to sound. 
In a digital environment, sound is stored according to rules defined by a codec. 
There are many different codecs, with different advantages and disadvantages, but all of them are necessarily discrete. 
In analog, this isn't true: AM and FM broadcasts are in some sense continuous represetations of the source signal. 

An ordinary radio tunes to a channel by filtering out everything but a narrow band of frequencies. 
The antiradio is, conceptually, the opposite of this: it filters out only one channel. 
This results in a wash of frequencies; if you played this signal into a speaker, it would just sound like noise. 
But it wouldn't be noise!
All of the individual signals would still be present. 
To take advantage of this, the antiradio then uses the filtered channel's signal as a filter on the combined signal.

This is a much more complicated and dynamic filter than a simple band-pass, of course. 
This project aims to execute this vision in real-time. 
This repository will serve as a proof of concept and testing ground for me to explore different codecs, DACs, and ways of creating fast audio filters. 
The final version will be a physical machine, so that it can make use of actual radio broadcasts in Seattle and be displayed publically. 
