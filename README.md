Project Outline
============

## Overview of Points
* Project Proposal = 10 pts  
* Vote = 5 pts
* Project Outline = 15 pts
* Meeting w/ Mike = 10 pts
* Milestone 1 = 25 pts
* Milestone 2 = 25 pts
* Halfway Check-in = 10 pts
* Milestone 3 = 25 pts
* Milestone 4 = 25 pts
* Final Outcome = 50 pts  
--> 200 Total

## Team Members
* Marc Simpson (marc.simpson@colorado.edu)
* Ian Ker-Seymer (i.kerseymer@gmail.com)
* Jake White
* Adrian Chen
* Mike Fyk
* Brian Newsom (brian.newsom@colorado.edu)

## GitHub Repo 
[As a way to share your project code and handle submissions, please create a GitHub Repo and place the link here so we know where to find your work]
https://github.com/BrianNewsom/CSCI4830-TrafficMonitor + Use Organization https://github.com/atlastrafficmonitor

## Project Sketch
[Use this section to sketch out the working parts of your project.  The project may change as you go, but try your best.  Describe how you intend to capture your data, clean it, analyze it, dump it, and vizualize it.  How will you set up your hardware?  What things are still uncertain and what things do you feel confident about?  What will be your process to get each of these things in working order?  How would you like your display to be 'triggered' in the installation?]
We intend to use IR sensors to monitor traffic through the doors. This can be accomplished by using two sensors to sense whether people are entering or leaving the building. Arduinos will run these sensors, and will write data to a file. The visualizations will read the file and create a visualization. In addition, musical notes will play everytime someone walks into the building. The visualization could be a line plot, or have a dot for every person in the building.

## Hardware
[This is a preliminary list; it will be finalized in a meeting with Mike (see below)]

    1. Kinect
    2. Raspberry Pi
    3. Infrared Sensor x4
    4. Central Server
    5. Speakers
    6. Monitor
    7. Arduino

## Roles
Given the varying expertise and interests, I'd like you to outline what team member will be responsible for what parts of the project.  It's okay if 2 people want to share certain responsibilities.  This is mostly for your own organization and, if things get rocky, so Mike knows who to talk to in the group.

Adrian, Marc - Hardware setup
Everyone - Algorithm to detect people
Ian - System administration of server, etc.
Brian, Ian - Sound
Jake, Mike - Visualization


## 4 Milestones
[Please list 4 Project Milestones you'll complete week-to-week to show your progress.  You will need to turn in some tangible example to prove you've completed 1 milestone each week.  Some combination of code snippets, data, screenshots, picture of the hardware setup, etc.  If these milestones need to change slightly, that's OK, as long as you tell Mike and Tom at least 2 days before submission (and as long as you haven't arbitrarily reduced the workload)]

1. Hardware, Sound, Visualization prototyping
    Do sound and visualization using any arbitrary data, get sensors working.
2. Algorithm to detect people
3. Integrate Hardware, Sound, Visualization prototypes
4. Setup project in lobby

    * Milestone 1: 
        - Visual: Some sort of D3 mockup that will interact with the data with sample data
        - Hardware: Skeleton code for collecting the data, go to Atlas a figure out logistics
        for wiring up the hardware
        - Sound: Get trigger inputs (socket API and keyboard input)
        
    * Milestone 2: 
        - Finalize algorithm for IR data, have live data streaming
        
    * Milestone 3:
        - First hardware setup, integration test.
        
    * MIlestone 4:
        - Do it live.
        
## Propose 3 Meeting Times
[You'll need to meet with Mike sometime during the week of 11/10 to finalize these details.  For this your whole team should try to be available for a **30 minute** meeting.  Mike is unavailable from 12-1 MWF and 12-2 TTh so don't propose those times.]
8:30 am Tuesday (sorry mike)

AND FINALLY... Remember to have fun!  This is going to be a challenging project, and there is going to be some tough hurdles, but it should be a good time if you get into it and get excited about what we're creating.  Mike will do his best to be available and around ATLAS so that in the evenings if students need to come in and work or try things, we can set times to do this.  Also we'll have a hardware expert [Abhishek Narula] from ATLAS who will help us in the process.  

Visualize 1 
============

Jake White and I (Mike Fyk) met to discuss visualizing people coming into the room. We decided that we would use circles to represent the number of people in the room. As the number of people increases, the hue of the circles changes from purple (low wavelength) to red (high wavelength), the size of the circles gets smaller, and the circles move faster. We found a great example with paper.js that displays circles with impressive collisions and allows us to control the size, speed, and color of the circles and we can write functions to update these values from the data. We are also considering overlaying text, estimating when the room is most likely to get less/more crowded, and showing past data/forcasted data below the visualization depending on our ability to implement these features. We have attached screenshots of the visualizations we made below.

Less Crowded:
![Less Crowded] (http://i.imgur.com/hDKWIXk.png)

More Crowded:
![More Crowded] (http://i.imgur.com/jfUQYbV.png)
