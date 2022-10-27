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

# 2022-25-09: Design Document Deaft w/ Jack & Alice:

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
