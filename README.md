# Dollo
a fully printed 3D printer, that scales.

# Goals in order of priority

1) Make a 3D printer that can make as many of its own parts as possible

2) Have it so the machine can scale with little to no throwing away of old parts

3) Make it easy to assemble

4) Use no more than a single 1KG spool of plastic to make.

5) Make it as low cost as possible.

6) use parts that are easy to find.

7) make it durable (since it can print its own parts this isn't super high priority)

8) hope people stop asking "what if you could 3D print a 3D printer" because of course you can and its not that unique of an idea

# Part count and list for small Dollo

(x=number of slots times 2) -- rack_x_units.stl

13 -- extention.stl

8 -- corner.stl

156 -- bow_tie.stl but extra never hurts

96 —- long_ties.stl

2 -- x_spacer.stl

6 -- motor_mount.stl

8 -- twist_corner.stl

4 -- large_gear.stl

3 -- gear.stl

4 -- middle_gear.stl

1 -- gear_one.stl

1 -- hot_end_mount.stl

Metal parts we hope to get rid of in the future

11 -- M3x40  for the motor mounts and bed gears

5 -- M3x10  for the motor mounts and bed gears

4 -- M3x20  for the z motor

4 -- M3 lock nuts  for the bed gears

Electronics and other

1 - main controller board (we use RAMBo and also like the idea of printing the pcb and solding the components your self)

3 - end stop switches   we are trying to come up with a clever way of doing with with printed conductive parts

5 - motors

1 - hotend or whatever tool tip you want really

1 - hobbed thing, gear or bolt

1 - bearing for extruder (might be able to print)

1 - heated bed

1 - glass/aluminum that fits on the bed

4 - springs and screw for leveling your bed.

Options for a larger printer

8 - extention_3_units.stl  This will make it so your printer can fit a normal heated bed in the normal way and not limit the space at all

4 - extention_x_units & more twist_corner.stl. You can add as many of whatever size you want pieces into the z axis, this print doesn't been anything extra for those to work

# How to assemble
1) start with the basic frame, take a single corner and butt joint all 3 extension pieces to it with all 4 bow_tie slots. then on the end of each of those add corner pieces then extension pieces again until you have built out a full cube shape.

2) put on the racks. first you need to decide what side you want to be up, this really doesn't matter since it should be the same on all sides. Once you have figured that out, you can start putting your slots on the top of your printer with more bow ties add racks on parallel sides and to the top of your remaining extension piece. each should have 3 racks on it.

3) mounting your motors. first you will need to put a gear.scad on your motor shaft, then you can take a motor and put the motor_mount_small on it and screw in the single counter sunk screw on the bottom using a M3x10 and then put it on your printer rack and make sure the gear aligned with the rack teeth. once it does you can keep it on the rack and screw in your other motor_mount_small to the other side. (make sure to do this on the printer because if you don't it wont go on after) do this for all 3 racks and make sure the motor faces out.

4) mounting the x axis. grab your x_spacer and put them on the end of what you already have assembled on the left over extention piece and then slide that into the motor mount on each side of the printer.

5) Get the frame ready for the bed. first you need to prep you printer by taking the crazy looking twist_corner pieces and bow tie them to the inside of the printers frame mirroring each other but keep the bottom one out on each side.

6) now take a motor and mount put the gear_one on it and mount that to your bed, then take your middle_gear and put those next to the motor and then put your large_gear and large_twist together, and put those next in line. 

7) putting the bed in. This can be kind of tricky, but you have to twist your bed so it goes inside the frame sideways and the you should be-able to twist it to make it fit in the frame with the corners sticking out. and this is why we didn't put in the bottom corner_twists, because now your bed sits just under them and once you have the electronics set up it will be able to twist into those and once its in the teeth you will be able to add your last parts under it.

8) Electricity is fun. take all of your motor and put them into the correct stepper controllers making sure that your Y motors are plugged in opposite of each other. Plug in your electronics and make sure to upload the correct Dollo version of marlin. Once you have done this you should be able to move your motors and this is where you move your z motor in the negative direction (negative because that make the hotend and the bed closer) and once it is up at the top, you can put your last twist_corners on your printer.

9) hot ends and end stops. at the point of making this commit I do not yet have the end stops figured out. But the hotend should put in your hotend mount and should just slide and clip into your x motor mount. 

10) setting up the extruder. Not sure what extruder we are going to use yet, but if you have done 3D printing before you should know how all of that works and be able to get it going.

Z options) I do have the z axis all modeled for being fully printed and able to scale

# Extra cool facts

1) I came up with the original version of this when I was 16 and in high school and it was done in blender because thats all I knew how to use

2) This printer as it stands is under 1KG of printed parts 

3) We printed the first Dollo on 3 Prusa Mendal printer that were printer on other printers them selves and so on, all the way back to the start, so these machine have only open-source in their genealogy

4) I lived 300 miles from the printer that I used and did all of the printing over the internet using octopi to print the first Dollo

5) The Dollo can (if you want) have a metal core structure, we built it in just in case and it saved plastic so it was a win win.

6) The Dollo was made by a me and my dad, I didn't the modeling and he helped me come up with ideas on how to fix the issues I has on the way, and he test fit most of the pieces (the printers were at his house)

7) The Dollo has swappable tool heads so you can mill metal parts if you want!

8) We had no plans on how this was going to work before starting. We have gone through probably close to a 50 different ideas on how this thing should even work.

9) Half way though we almost gave up on the z and made the Dollo a Delta style printer (might still have something like that in the future)

10) We looked at a lot of other peoples printer before we could figure out how to do this one, we really could not have done it with out the community.
