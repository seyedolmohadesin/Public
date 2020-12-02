## Running a Microfluidic Experiment

- [What you need](#what-you-need)

- [Setting up the syringes](#setting-up-the-syringes)

- [Preparing the microfluidic chip](#preparing-the-microfluidic-chip)

- [Turning on LAMBDA](#turning-on-lambda)

- [Loading a worm](#loading-a-worm)

- [Imaging brain activity](#imaging-brain-activity)

- [Imaging another worm](#imaging-another-worm)

- [Shutting down](#shutting-down)

- [Cleaning up](#cleaning-up)


### What you need

- Syringe reservoirs
- Buffer and odors 
- Microfluidic chip
- Loading syringe
- Not seeded agar plate
- 25 mM levamisole
- Imaging plate
- Scotch tape
- Pipette tip box
- Waste beaker
- DI water
- Centrifuge tube

<img width="802" alt="Screen Shot 2020-06-22 at 8 14 17 PM" src="https://user-images.githubusercontent.com/43148819/85346931-0396e880-b4c5-11ea-9799-362889e575f1.png">


### Setting up the syringes

- Position the black knobs horizontally for all of the syringes to block air flow. 
<img width="200" alt="Screen Shot 2020-06-22 at 1 02 14 PM" src="https://user-images.githubusercontent.com/43148819/85315214-9d8c7000-b488-11ea-95e1-7c3bdf0e8d34.png">

- Check pressure on the perfusion system, it must be between 3-6 psi. 
<img width="200" alt="Screen Shot 2020-06-22 at 5 42 11 PM" src="https://user-images.githubusercontent.com/43148819/85338152-bfe5b400-b4af-11ea-9b59-44d05ecd6e66.png">

- Place the buffer syringe and odor syringes on the perfusion system rack, make sure stopcocks are in horizontal position.
- Fill each syringe reservoir with the corresponding odor/buffer. 
- Fill the two syringes labeled with "diH2O" with DI water.
- Note: Do not fill syringes over 25 ml.
- Label each tube with its valve number by using a tape, don't tape the label too close to the tip of the tube.
<img width="200" alt="Screen Shot 2020-06-22 at 5 59 45 PM" src="https://user-images.githubusercontent.com/43148819/85339461-2f5ca300-b4b2-11ea-9584-526531a42baf.png">

- Cap each syringe with its metal stopper and secure it. 
- On ValveLink controller turn on the valves that you are going to use during the experiment 
- Gently insert the flexible tubing into the pinch valve for each syringe.

**Do the following steps for each syringe separately:**
- Position the black knob vertically to turn on the air pressure. At this point the stopper may pop up, if that happens secure the stopper again and make sure there isn't any pressure leak.
<img width="200" alt="Screen Shot 2020-06-22 at 6 07 45 PM" src="https://user-images.githubusercontent.com/43148819/85340017-4fd92d00-b4b3-11ea-8a79-e4e4a56edff8.png">

- At any point during this procedure you can make sure there isn't any pressure leak by reading the pressure on the perfusion system, if there is a drop in pressure make sure all the stoppers are secured. 
- Hold the tip of the tube into the waste beaker and turn on the stopcock, don't let the tip of the tube touch the waste.
- Let the fluid flow for about 30s and until there isn't any bubbles in the tube. 
- Turn off the corresponding valve manually by the controller, the flow must stop immediately, if not make sure the flexible tubing is inserted correctly into the pinch valve and try again.
- Place the tube into the pipette tip box.
- Repeat the above steps for the remaining syringes.

### Turning on LAMBDA
On the right PC:
- Open a command line window and type ```lambda```, wait until you see ```dragonfly is initialized```.
- In [modes.json](https://github.com/venkatachalamlab/venkatachalamlab/blob/master/protocols/lambda/microfluidic_system.md#modesjson) file define a new mode for your experiment and set the parameters. 

On the left PC:
- Open a command line window and type ```valve_controller```.
- Open another command line window and type ```stage```. 
- Open Zaber software and set the unit to um.
- Open Lense Driver Controller software


### Preparing the microfluidic chip

- Tape chip to the imaging plate and place it under the dissecting microscope.
<img width="200" alt="Screen Shot 2020-06-22 at 6 20 32 PM" src="https://user-images.githubusercontent.com/43148819/85340965-26b99c00-b4b5-11ea-9f20-bbe7f08c5253.png">


**Do the following steps every time that you want to insert a tube into the chip:**
1. Hold the tube into the waste beaker.
2. Turn on the valve manually by using the controller and let the fluid flow for couple of seconds, make sure there isn't any bubbles left in the tubings.
3. Turn off the valve.
4. Rinse the tip of the tube with water.
5. Don't touch the tip of the tube.
6. Insert the tube into the chip.

- Insert the buffer tube into the chip's waste channel and turn on its valve via the controller.
<img width="200" alt="Screen Shot 2020-06-22 at 6 28 48 PM" src="https://user-images.githubusercontent.com/43148819/85341469-42717200-b4b6-11ea-821d-dace00c24f68.png">

- Let the buffer wash the chip for couple of minutes, use the vacuum tube to suck any liquid that comes out of the channles.
- In the meanwhile check the chip for any leak or damage, you should see liquid coming out of all the channels including the worm trap.
- Turn off the buffer valve and remove the tube from the chip.
- Insert each tube (Make sure to follow the steps above for inserting the tubes) into its corresponding chip channel.
- Turn on control1 and buffer valve.
- Turn on each odor valve and let it run for about 5 seconds and then turn it off.
- Turn on control2 valve (control1 and buffer are still on).
- Tape the vacuum tube next to the waste channel to suck the waste.
- Let the three fluids flow for couple of minutes and until there isn't any bubbles in the chip.
- This is called a **clean cycle**, it cleans the chip from odors and removes the bubbles.
- Tape all the tubes to the plate to secure them.
<img width="300" alt="Screen Shot 2020-06-23 at 4 12 06 PM" src="https://user-images.githubusercontent.com/43148819/85455909-698a7b00-b56c-11ea-9c09-e46eb0bd6109.png">

- Turn off all the valves and carefully put the plate aside.

### Loading a worm

- Clean the loading syringe thoroughly with diH2O under the sink.
- If you intend to use levamisole for better immobilization of the worm, mix 3 parts buffer with 1 part 25um levamisole in a centrifuge tube to a total of 10-15 mL. If not, only pour 10-15 ml of buffer into a centrifuge tube.
- Place about 5 worms on a not seeded agar plate.
- Turn on the clean cycle. 

**Every time that you want to use the loading syringe rinse the tip of the tube with DI water**

Following steps are done under the dissecting microscope.
- With the loading syringe slowly pour 2ml of buffer mixture on the worms.
- Fill the syringe halfway with buffer mixture, place the tip of the syringe in the buffer that is in the plate, empty the syringe a little bit to get rid of the bubble at the tip of the syringe and then very slowly suck the worms up the loading syringe one by one. 
- The last worm should be very close to the tip of the tube.
- In the process of loading worms make sure you don't suck air into the syringe.
- Carefully insert the syringe into the worm channel.
- Slowly push the syringe until you see a worm coming in. 
- By applying positive and negative pressure orient the worm the way you want (head in front or tail in front).
- By applying enough pressure load the worm into the worm trap in a way that the worm's nose is slightly out of the channel.
- If there is any problem with the first worm, push it out of the channel and try to load the next worm in the syringe. 
- If bubbles appear in the chip wait couple of minutes until clean cycle removes them.
- Note that during this time clean cycle was on to ensure that bubbles don't get stuck in the chip.
- Leave the syringe in the chip and slowly move the imaging plate to the confocal microscope.

### Imaging brain activity

- Add a drop of oil to the chip, try to drop it on top of the worm channel.
- Slowly place the imaging plate under LAMBDA (Be careful about the tubings).
- Turn on the LED all the way up.
- Use the Xbox controller to approximately center the worm.
<img width="300" alt="Screen Shot 2020-06-23 at 4 27 59 PM" src="https://user-images.githubusercontent.com/43148819/85457914-87f17600-b56e-11ea-9493-36d6b5026b7e.png">

- Use Zaber to slowly move the stage upward.
- Stop the stage right before the oil touches the objective.
- Move the slider in the lens driver software to the right until chip channels appears in the bottom microscope.
- By using Zaber move at 10um/s velocity until the oil touches the objective.
- Use the xbox controller to center the worm in bottom microscope.
- Turn down the LED.
- On lambda command line window type ```DO set_mode widefield```, then type ```DO start```.
- By using Zaber focus on the worm.
- Use the xbox controller to position the worm perfectly.
- Use Zaber and go backward at 2um/s velocity for about 5 seconds to focus on the bottom of the worm.
- For imaging OH16230 type ```DO set_mode color```, and then type ```DO start```.
- When the imaging starts type ```DO _start_runner <mode>```.
- On the ValveLink controller or the perfusion system you must see that some valves change their status.
- You can see the status of the valves in valve_controller command line window.
- Wait until it says ```runner: experiment has ended``` and then type ```DO stop``` to stop imaging.
- Copy and paste the data to an appropriate folder in NAS.
- Note that you can only copy the log file after you shutdown the microscope.
- When you are done with imaging the worm, push the worm out of the channel by applying pressure to the syringe, don't do this aggressively.
- Use the bottom microscope to make sure that the worm didn't get stuck in the channels.

### Imaging another worm

- If there is still worms in the syringe you can load them and image them.
- If not, you can fill the syringe with few worms and try to load them by using the bottom microscope.
- Or you can remove the imaging plate and use the dissecting microscope to load another worm.

### Shutting down
- Type ```DO shutdown``` on lambda command line window and wait for about 1 minute.
- Type ```DO shutdown``` on stage command line window.
- Close all the command line windows.
- Copy and paste the log file to your data folder.
- Close Zaber and Lens driver software.
- Gently clean the oil on the objective using lens paper and alcohol.

### Cleaning up

- Remove all the tubings from the chip.
- If you want to reuse the chip in near future insert one of the control tubings which is filled with water into the chip's waste channel and let it run for 1-2 minutes to clean the chip.
- Clean the oil on the chip using kim wipes and alcohol.
- Empty all the syringes to the waste container except for the two control syringes.
- Turn on the pinch valves that you were using by ValveLink controller and remove the flexible tubings from the pinch valves.
- Turn off the valves.
- If you don't plan to repeat the experiment the next day Remove all the syringes from the setup.
- Clean the loading syringe and place it into it's box.






