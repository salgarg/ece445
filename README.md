# ECE445 - Saloni Garg's Lab Notebook

# 2022-08-29: Meeting with Alice and Jack

- In this meeting, our objectives were to introduce ourselves to each other and talk about project ideas for the semester, as well as our technical backgrounds. We discussed the project ideas posted on the web board by Alice and Jack, including a remotely adjusted cast similar which would essentially add remote capabilities to existing AirCasts and a phone case that converts energy generated by a crank to charge the phone. I learned that Alice has experience with frontend software development, and Jack has experience working in networking and with microcontrollers. 

# 2022-09-11: Project Proposal Draft with Alice and Jack

- In this meeting, I met with Alice and Jack to discuss our project proposal, which is due this upcoming Thursday and will be minorly reviewed by our TA during class time on Tuesday. We worked together to come up with the 3 high-level requirements associated with our project. Along with this, we worked together on LucidChart to develop the block diagram of our project components. We want to confirm that we did this correctly and remembered to include everything necessary when we meet with our TA on Tuesday (2022-09-13). We also split up which portion of the ethics and safety section of the proposal that we would each work on, hoping to have all of it done by Tuesday or Wednesday so that we can discuss our proposal overall before the deadline on Thursday.

## First Draft of Block Diagram:

<img width="429" alt="image" src="https://user-images.githubusercontent.com/41525737/189682936-fc0ad3cd-7a70-4eac-94d3-4468b77c0259.png">

# 2022-13-09: First meeting with TA

- Alice, Jack, and I met with our assigned TA for the fist time, to introduce ourselves, go over our project proposal draft, and get some tips on how to move forward with our proposal before the deadline. We showed our TA which microcontroller we were thinking about using: https://www.adafruit.com/product/5400, and he explained to us that we would have to purchase just the microcontroller portion of this, and that we should avoid de-soldering it to extract that component. We found the component being sold separately here: https://www.adafruit.com/product/3320.

# 2022-15-09: Project Proposal cont. with Alice & Jack

- Discussed and researched which microcontroller to use for our project and finalized ESP32 from Adafruit - as it has bluetooth capabilities too + was discussed in first meeting with TA as a common choice
- Discussed the requirements we should have for each subsystem and how to qualify/quantify them for the project proposal write-up
- Discussed how to come up with a mathematical analysis which we could apply to our risk tolerance analysis. We emailed the TA to see about how we could approach this and he suggested calculating the torque of the motor needed to adjust the strap tightness on the cast, and proving that this is possible with the motor we wanted to utilize. After doing some more research on types of motors we could use, we found one that sounded reasonable and performed the necessary calcualtions. In addition to this, Jack added a portion to the risk tolerance analysis regarding the stretch risk of the system's pressure module. He did the research and calculations for this part as well to prove the pressure module will work with our procedure.
- Finalized our block diagram as per the TA's suggestions

## Finalized Block Diagram for Project Proposal:
![image](https://user-images.githubusercontent.com/41525737/190554209-e7aa88ed-e8d1-4fd5-beae-b8369b8c3e5e.png)

# 2022-16-09: Initial Meeting with Machine Shop:

- At this meeting, Jack, Alice and I met with the machine shop to go over our design idea, and receive feedback. We were provided with feedback on the feasibility of our two functionality ideas - automatic strap adjustment using a motor attached to the straps of the cast, as well as the air cell inflation/deflation. We were told that it would not be feasible to adjust the pressure level of the air cells, and that we should stick with just utilizing a pressure sensor and have the user pump the air cells in the original method (attached air cell pump) until we reach the pressure value specified by the patient's doctor. Additionally, the machine shop representative shared multiple methods of mounting our PCB and motor to the air cast, such as attached the motor directly to the strap of the cast, and potentially having the PCB stored in a compartment with a belt loop attachment, such that it does not make the cast itself too bulky. Furthermore, the representative mentioned that the machine shop works on a first come first serve basis, so we should keep that in mind for the future when we need work done by them.

# 2022-22-09: Meeting #2 with TA:

- Discussed feedback from project proposal including the values which are not necessary within subsystem requirements, and positive feedback on our tolerance analysis portion
- Shown around the lab that we have access to, and what different types of parts we can borrow from the lab rather than purchasing ourselves
- Discussed what the design document should look like in relation to the project proposal - more detail than the project proposal but similar general concepts, with the addition of cost analysis.

# 2022-25-09: Design Document Draft w/ Jack & Alice:

- Worked together to finalize the components necessary for the design document prior to the design review on Monday, 9/26
- Understood that this was a rough draft which would need to be edited based on feedback received during the design review, prior to the final deadline on 9/29. 

# 2022-26-09: Design Review #1 w/ Prof and TA:

- Presented design document to Professor Flifet and several TAs, outlining our problem/solution, high-level requirements, visual aid, block diagram, subsystem breakdown, cost/schedule analysis, tolerance analysis, ethics/safety information, and citations
- Received feedback to improve our visual aid with more detail, clean up our block diagram in order to make it more clear which parts are connected and remove the "boot" element from the diagram altogether, be more specific in our subsystem requirements to ensure we are not just repeating specs of the component but rather requirements of our design and including more citations to back up our document overall

# 2022-29-09: Meeting #3 with TA + Design Doc Finalization:

- Discussed several questions regarding the design document with our TA, which were discussed amongst Jack, Alice, and I prior to the meeting through text and comments on the docmument itself
- Received clarification on how to improve with our subsystem requirements, block diagram, and high-level requirements 
- Worked remotely to improve the design document based on professor and TA feedback in order to submit the final document prior to the 9/29 11:59pm deadline
- Link to final design document: https://docs.google.com/document/d/1LdknCm0zml1bBu3zVbliBF07CaJqPWh1cXvjo9yShkY/edit?usp=sharing

# 2022-03-10: PCB Design Tutorials [individual]:

- Viewed the following tutorials to have more insight (outside of the KiCAD tutorial from the start of the semester) on how to design and build a PCB, what to keep in mind, how to troubleshoot, and how to order the design on PCBWay:
  - https://www.youtube.com/watch?v=ia2n7P3Csac
  - https://www.youtube.com/watch?v=nIGwmF8dId0
  - https://www.cirexx.com/pcb-design-steps/

# 2022-10-10: Schematic + PCB Design Continuation:
- Met with Jack and Alice to review our finalized components for the design, and move forward with building out a full schematic, such that this could be converted to the PCB design
- Discussed which motor should be finalized along with a motor driver which would both be compatible well with ESP32 and Arduino IDE 
- Read through documentation for instructions on connecting motor drivers, motors, and ESP32 as well as on which ESP32 ports were meant for ADC and whether this was necessary for the purpose of our project

# 2022-11-10: PCB Design Continuation [individual]:
- With the finalized schematic of our design completed by Alice and Jack - as they attended the PCB Design Review conducted by TAs and Instructors (I had a personal conflict) -- we were able to convert this to a loose PCB design using footprints provided through KiCad as well as from online downloads for the ESP32 footprint
- Routed the PCB tracks based on KiCad suggestions and feedback from PCB design review 
- Made sure to keep tracks connected to power and motors thicker 
- Tried to keep all components and routing in a frame of 100mm x 100mm or less as per the course requirement for PCB design 
- Did not complete routing as I was having trouble with some, discussed potential solutions/fixes to the routing with Alice and Jack 
- End result on my end was as follows [incomplete]:
<img width="672" alt="image" src="https://user-images.githubusercontent.com/41525737/195450921-7a0b9b85-7ca5-4057-8452-7edd32b29b9b.png">

# 2022-12-10 & 2022-13-10: PCB Design Finalization and TA Meeting #4:
- cleaned up PCB design routing to make it cleaner and ensure it fit the necessary widths + hole sizes for PCBway 
- met with the TA and found out we had some hole sizes that were too small, causing our PCB to cost ~$60, to mitigate this issue we removed unnecessary grounding holes that were in the ESP32 and motor driver footprints
- final PCB design was as follows:
<img width="692" alt="image" src="https://user-images.githubusercontent.com/41525737/196776381-c3514bcc-4e99-4203-a326-91957290c6c4.png">

# 2022-16-10: Ordering parts:
- Met with Jack and Alice to order the parts we finalized for our design
- Had to ensure that the parts were available and switch to others if they weren't
- Had issues with availability of exact motor driver we were originally looking at (DRV8833PWP) but were able to find a very similar one which would not affect our overall design or PCB, which was in stock (DRV8833PWR)
- Did not order the Molex 4-pin cables or battery pack yet, as we are waiting to order these until we talk to the machine shop about where everything will be placed on the boot and how it will affect the weight of the boot 
- The following day all of our purchase requests were approved! 

# 2022-10-27: Meeting #5 w/TA + Meeting with Machine Shop:
- Received parts ordered previously and locker to store parts
- Notified that PCBs would arrive soon (within a day or two hopefully)
- Notified that the soldering assignment is most likely not a requirement anymore/might be extra credit later in the semester
- Discussed Alice's start to the UI of our project, which includes basic stats and buttons as of right now
- Met with the machine shop to show them to motors we received and the boot, and hand off the parts for them to assemble 

# 2022-11-02: Working Session with Alice and Jack
- Met with Alice and Jack to pick-up our PCB boards and begin work on our project
- Found necessary resistors and capacitors for our motor driver circuits and pressure sensor modules, with the exception of a 0.2 ohm resistor which we could not find in the lab
- began soldering of resistors onto PCB - jack completed the direct soldering portion while Alice and I observed, learned how to do this so that we can do some of it in the future, and helped to organize the materials/tools necessary to do the soldering
- completed soldering of 2 resistors for the pressure sensors on the board

# 2022-11-03: Meeting #5 w/TA + PCB Re-design
- Met with Staisu to discuss progress on design module testing and overall project progress
- Discovered the need for a programmer circuit within our PCB design, which was missing from the original design
- Spent quite a few hours implementing the following programmer circuit suggested to be used with the ESP32 microcontroller, with auto-programming capabilities: https://pcbartists.com/design/embedded/esp32-cp2102-programmer-schematic/, re-routed the PCB for additional components, ensured we did not have holes on the design which were too small, and that the new additions to the PCB design did not cause it to fail the PCBway audit
- Submitted the new PCB design for order, expecting it to arrive prior to the final demo
- Discussed potential back-up plan in case the PCB does not arrive in time to work on and test prior to the final demo, as thanksgiving break is right before the demo and all three of us will not be on campus if the PCB arrives during break - and settled on the possibility of breadboarding the ESP32 dev kit and utilizing the programmer from it to interact with the ESP32 on the original PCB boards 
- Began testing with ESP32 Development Kit -- tried to simply get it working with the Arduino IDE - ran into some issues with the cable we were using as it was microusb but not a wire which could carry data, so we had to use a different wire until successfully getting the ESP32 to transfer data to our computers and complete a simple LED blinking test
- Placed order for multiples of original components necessary for design in order to have backups, and for new components needed for programmer circuit 
- Also placed order for motor driver breakout board in case the programmer circuit on the new PCB boards is not usable in time, such that we can still control our motors without full integration on the PCB
- The following is the updated circuit schematic and PCB design for our project:
<img width="806" alt="image" src="https://user-images.githubusercontent.com/41525737/200968657-201494e5-83f7-4f2a-a6a4-22a53d29aac9.png">
<img width="588" alt="image" src="https://user-images.githubusercontent.com/41525737/200968693-1a0e35e3-e8cd-48a3-b67a-d63b6c8f0e32.png">

# 2022-11-04: Working session with Alice and Jack [Motor subsystem]
- began testing on motor subsystem
- since the motor drivers we are using with the esp32 can only be on the PCB, we needed to find motor drivers available within the lab room which would still be compatible with the stepper motors we are using, as well as the esp32 development kit in order to properly begin testing the code to control the motors, motor speed, and torque applied by motors -- we found online sources outlining the capabilities of L293D motor drivers with our Nema-23 stepper motors, and were able to successfully breadboard our motors and motor drivers with the esp32 development kit
- Some of the sources used for breadboarding the L233D motor drivers with our Nema-23 stepper motors and the ESP32 dev kit were as follows:
https://microcontrollerslab.com/stepper-motor-l293d-motor-driver-ic-arduino-tutorial/
https://www.hackster.io/Arnov_Sharma_makes/l293d-with-esp32-wemos-lolin-d32-v2-hacked-edition-ea2086
- had to find specifics about the Nema-23 motor such as the revolutions per minute possible for this motor
- we were able to get the stepper motor working at a speed of 60 RPM by the end of this session

# 2022-11-07: Working session with Alice and Jack [Control and Pressure Subsystems]
- Began working on bluetooth communication between the serial monitor of the Arduino IDE, a serial bluetooth terminal, and the ESP32 using the ESP32 Development Kit
- Tested the bluetooth communication with the computer through the serial bluetooth terminal, by programming a LED turning on/off based on input to the serial bluetooth terminal containing the letter A or B -- found success with this test so we knew the bluetooth comm was functional
- Continued pressure module testing to display pressure values read by FSR through bluetooth serial terminal - had issues with this due to baud rate but after researching and fixing this issue we were able to get the pressure values to display both on the bluetooth terminal and the serial monitor
- Had another issue with stack dump if pressure sensor was pressed too hard beyond its limit of reading - fixed this by setting a maximum pressure limit that could be ready and displayed within the code (need to go back and ensure this does not mess up the values calculated after this/error testing overall)

# 2022-11-08: Working session with Alice and Jack [Pressure and Motor Subsystems]
- Tested the pressure module further to determine if pressure values being read were consistent, found some issues where the sensor is reading pressure values when there is no pressure being applied to the sensor -- need to go back and check on this issue and test with more consistent weights rather than manual pressure applied with fingers
- Attempted to control motor speed using RPM values, such that we knew the torque being applied by the motor based on the speed it was running at - we ran into an issue here where the RPM does not seem accurate to the value that we are setting, and is somewhat incapable of going at a speed greater than 100 RPM - explored various different options for solving this issue or ensuring that we are receiving the correct RPM output through the motor but this still requires further testing and attention overall
- Used the following graph found specifically for the Nema-23 for a torque vs speed relationship:
<img width="848" alt="image" src="https://user-images.githubusercontent.com/41525737/200969961-a5d1b613-1631-4a7e-b78a-6ebcbf3aef87.png">

# 2022-11-09: Working session with Alice and Jack [Control Subsystem]
**Kept track of work done beyond this point in a notion page linked here: https://marshy-foe-bb6.notion.site/445-lab-notebok-updates-bada172fb9d5457fbcb62aa42e90c2dd - but rewrote here in a refined manner

- Worked on bluetooth characteristics -- communicating pressure value to phone as client and esp as server in HEX - need to figure out how to do this in ascii and then move communication protocols to web app
- having issues connecting to wifi from web app altogether
- practiced soldering so that we will be prepared when new PCB orders come in

# 2022-11-10: Meeting #6 w/ TA + Working session with Alice and Jack [Pressure and Control Subsystems]
- Had a weekly meeting with Staisu about parts we've been using and our progress with testing them, the lack of points for anything in the gradebook, and the difficulty of implementing bluetooth functionaliity for the UI we had created, since it is a web app using React rather than React Native (meant for mobile web apps, which has more available guidance on implementing for the bluetooth functionality of the ESP32
- Worked on pressure module and integrating the measurements of pressure between the wall of the AirCast and air cell with the UI
- Decided to switch to using WiFi communication betweenn the ESP32 and UI, as it is simpler to implement and has more resources available online, and can still perform the same functionality as originally intended

# 2022-11-11:

testing pressure module with wifi and UI with wifi, found out our ADC pins have been getting too much power and are fried on the esp32 dev kit - worked with TA and used oscilloscope + multimeter to figure this out - this is why the values of the pressure module were very inaccurate

# 2022-11-12:

tried to use just the esp32 microcontroller not the dev kit to program using the programmer breakout board found in the lab - tried both on PCB and with wires directly soldered onto esp32 — realized we needed buttons or transistors to put the esp32 into bootloader mode/not after the program was loaded - didn’t have any buttons so tried just doing this by quickly removing certain wires from ground based on if they were active high/low and what was necessary to put them into bootloader mode 

# 2022-11-13:

continued testing uploading code with getting accurate reedings with “spider” - found buttons and set up circuit but consistently got issue with stuck in download mode, received new esp32 dev kit and began testing pressure module further with this

# 2022-11-14:

received new PCB - began soldering, found out we were previously using the wrong pins of the esp32 for the pressure module causing the esp32 ADC pins to get fried, continued testing pressure with new dev kit

# 2022-11-15:

mock demo with TA, received boot from machine shop all put together, got motors and pressure module to work correctly with dev kit, worked on motor code, continued soldering pcb components, struggled with micro usb component on pcb, after soldering - ssp32 was getting power but could not be recognized by arduino - need to investigat this issue further, but micro usb component broke off - hard to solder

# 2022-11-27:

tried to integrate motor with pressure code — while controlling speed of motor based on a button toggle in frontend - reaching a kernel panic while trying to control motor and it stops working — going to continue trying to get both to work together tomorrow

# 2022-11-28:

successfully got motor code working alongside pressure module - without crashing, using the frontend interface. this is all being done using the breadboard & boot & esp32 dev kit, not the PCB as that does not currently work. We plan to make sure our code + modules are fully integrated aside from the PCB before trying to make the PCB work further with subsystems integrated within it, tried to start brainstorming ways of still integrating as many subsystems as possible with PCB rather than breadboard - including bodge wiring the esp32 dev kit to the esp32 footprint of the PCB, and integrating all other modules within the PCB directly OR bodge wiring the TX and RX transmission line traces properly such that data can be transmitted with the new PCB version using the programming circuit and esp32 chip itself rather than the dev kit
