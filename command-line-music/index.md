---
layout: inner
title: command-line-music
permalink: /command-line-music/
---
<script src="http://api.html5media.info/1.1.8/html5media.min.js"></script>
<br>
<div align="center">
<h3>Composing Music with Nyquist SAL</h3>
</div>
<br>
<div align="left">
During my time at Carnegie Mellon University, I studied under Roger Dannenberg, professor of computer science, art and music at CMU, as well as the lead creator of Nyquist.
Nyquist, 
found <a href="https://www.cs.cmu.edu/~rbd/doc/nyquist/part2.html#2">here</a>, 
is described as "a language for sound synthesis and music composition. Unlike score languages that tend to deal only with events, or signal processing languages that tend to deal only with signals and synthesis, Nyquist handles both in a single integrated system." This means that signal processing and sound synthesis in Nyquist is more akin to writing programs in Python than it is to creating music with a digital audio workstation (DAW), like GarageBand.
<br><br>
To create my composition using Nyquist, I started with the nineteen second sample loaded into the nyquist IDE, playable below.
<br><br>
<h4>100 Grandkids, Mac Miller</h4>
<br>
<audio src="audio/100-grandkids-sample.mp3" controls preload></audio>

<br><br>
In order to create the sounds in my final composition, I employed numerous signal processing techniques such as sound-stretching, amplitude modulation, and low-pass filters. Additionally, the creation of my composition was primarily executed using 
multiple functions like the <i>Load Sample</i>. For those unfamiliar with Nyquist's coding syntax SAL, the Load Sample function reads the wave file, plays it backwards, stretches the sample by a given value, and sets its volume with amps. For those familiar with python and other common programming languages, these functions may be readable, although syntax is distinct from more widespread languages.
<br><br>
<p class="text-center"><strong><i>Load Sample Function</i></strong></p>
<img class="img-responsive" src="img/ls-and-bs-functions-1320x668.png" title="Functions in Nyquist">
<br><br>
This is how interaction with nyquist is, and how the composition was created. Interestingly, the techniques used to process and synthesize sounds are no difference from graphical interfaces other softwares like GarageBand, althought this format offers greater control over the produced sound. It comes at an obvious cost of having to code your actions instead of manipulating the sound more interactively. 
<br>
<br>
In the end, my composition "Elevator Service" was created by running a simple function
<mark>play sim(sound(comp()) * 0.7, sound(make-beat()) * 0.7)</mark>. Functions <mark>comp()</mark> and <mark>make-beat()</mark> are functions that call other functions. To see this in more detail, view <a href="https://github.com/Sebastian-O-Rodriguez/about/tree/master/command-line-music/comp/comp.sal">the full composition</a>, written in SAL.<br> <br>
<h4>&emsp;Final Composition</h4>
<br>
<audio src="audio/elevator-service.mp3" controls preload></audio>
<br><br><br>
</div>