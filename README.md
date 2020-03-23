# Seven Pleasures of Pris
Improvising Ai robot duo modelled on ev2: an improvising drum and sax duet (Craig Vear and Jonathon Eato)

Album available at https://patabots.bandcamp.com/album/seven-pleasures-of-pris

The music in each of these tracks was created with artificial intelligence and machine learning. You will hear two AI-Bots: one in the centre uses soprano sax samples as its source, the other in wide stereo uses percussion. The two AI-Bots were programmed to respond to the other's sound and to contribute to the ongoing improvisation live and in realtime. 

Each AI-Bot is controlled by its own AI and is working without any human intervention. They are listening to each other and co-creating, and crucially doing something in the music that is beyond mimicry or behavioural response. 

The AI underpinning each Bot is driven by several Creative AI datasets and Machine Learning using a special process called embodied intelligence. The datasets are derived from real human musicians improvising with an AI-Bot. The AI operates on several concurrent processes: 
1) raw data from the live music 
2) dataset records of previous live improvisations 
3) statistical correlations using multi-level perceptual neural-networks 

These are then controlled by an affect module that responds to the dynamics of the live improvisation and manipulates a gate system that recombines these streams into a final data flow. It is this that is used to drive the wheels of the physical bot and trigger the sounds. The affect module, containing triggering, routing and smoothing, are the three most important methods in this whole system. It is important that all the other elements are built using data and symbolic algorithms from inside the embodied relationship of musicking. But these methods are the core of what I understand it is to do musicking:
1) listening
2) having my own train-of-thought
3) being surprised and maybe doing something with that
4) being surprising

credits
released December 2, 2019 

Thanks to Jonathon Eato for his kind permission in letting us use the recordings of his saxophone as source material for this album.

## About the Code

The Max patch controls the wheel movement and sound generation of a single robot in the duet. A seperate python script controls the robot movement through OSC data transmission from this main patch.

The AI embedded in this patch is based on the principle of Embodied intelligence in which the AI behaviour inside the domain of musicking is perceived to be creative and co-operative.

The patch is listening to the other robot, so a cross matrix will need to be constructed with the sound from one laptop becoming the input for the other, and vice versa.

The AI is also embedded with three types of machine learning: the first a bank of neural nets (traditional statistical ML), the second data queries from raw captured data of a musician improvising with these robots,  and the third a short-term audio-memory buffer.

Together these three learning components represent:
1) learnt instinctual response (Neural Net)
2) performance technique (raw data set)
3) thematic musical material (short-term memory buffer)

A "Turing Test" of this approach to AI is only to be felt inside the musicking.


## Setup
* 2 laptops each running a version of the AI software in Max:1) /seven_pleasure_of_pris_vear.maxpat; 2) /seven_pleasure_of_pris_eato.maxpat
* 2 robots each listening to OSC streams from the laptops. I used 2x GoPiGo piggy backs ontop of Raspberry Pi. The robots do not do any other processing other than translate the wheel Left and wheel Right data into physical movement of the robot.

I have included the machine learning environment and all the datasets. The datasets weere formed using the follwing features: ID, kinect_limb, x, y, z, audio_freq, audio_amp

All other details are embedded into the patch.
