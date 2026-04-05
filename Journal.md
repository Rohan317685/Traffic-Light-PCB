
# First Journal

I spent 3.5 hours on the schematic and I used lapse but I didnt press record so I decided to just journal:

[I Read the NE555 Datasheet](https://www.ti.com/lit/ds/symlink/ne555.pdf?ts=1775224237326)

I made a schematic but it was really bad because there were so much overlapping with the wires and it was very cramped, heres a image:
![Image](https://cdn.hackclub.com/019d580f-5a4c-7b69-92bf-6f5cec681412/20260404_02h41m49s_grim.png)

I ended up not using the circuit since it  was not very readable and wiring overlapped a lot also I couldn't even read it so that wont work out, I decided to use a lot less cramped schematic and reference since in the previous one d1 led was being clipped of by the wiring and a lot of designators werent readable and in U2 everything was overlapping.

It also took me a while to make the schematic because i used the ne555D and i was supposed to use the Ne555p because ne555p is tht (through hole technology) and the ne555d was surface mount which makes it a lot harder to solder. The ne555d also uses a Soic-8 package type and a ne555p uses a PDIP-8 package. THe ne555d was very compact however it required reflow soldering which i cant do. 

The new schematic I made makes it a lot more easier to read, there is far less overlapping and you can read most of the designators properly however it's not perfect and you cant read a few designators like r5 which overlaps with the wiring and I fixed that in the third journal! I also faced a couple of issues regarding the errors, I tried using pwr flags but for some reason the errors refused to disappear and when i placed 2 pwr flags it started complaining even more and when I kept a pwr flag at the source it still complained that there was no power input to gnd so I decided to ignore the errors.

[I Referenced this circuit since it was a lot more cleaner and the pins were the same as in kicad](https://eleobo.com/traffic-light-circuit-using-555-timer-ics/)

![Image](https://cdn.hackclub.com/019d5829-66ee-7bb3-ad3e-72197a4fdcb1/20260404_12h03m09s_grim.png)

# Second Journal

I spent 1.5 hours:

I made the PCB! It took a while because I still had to find the footprints and it wasn't to hard I used lcsc to find the footprints for their resistors capacitors and chips. I also found a easier way to fillet edges! I was manually cutting the line edges and using the circle tool to fillet it however I did right click -> shape modification -> fillet lines. I realised I could do that after @alexren mentioned it in her channel.

I made it compact and I centered it to make sure they were as similar to actual traffic lights as possible, I had to slightly move them because there wasnt enough space for the "traffic lights" silkscreen so its not perfectly centered but its somewhat accurate.

I also had to find a proper connector because I was thinking of changing the schematic to have a usb port but then realised a simple 01x02 connector and a 9v battery would do the job and I didnt want to over complicate it also the standard usb-c gives 5v and I needed 9v so if I did choose for a usb-c port I would've needed a different scaled version.

![Image](https://cdn.hackclub.com/019d5873-bbb7-7d49-9dcf-b64a9994dfec/20260404_13h22m01s_grim.png)

![Image](https://cdn.hackclub.com/019d5874-5ee7-74c7-9828-98bfcc7216e3/20260404_13h22m11s_grim.png)

![Image](https://cdn.hackclub.com/019d5874-bd05-709c-9ba1-b99bfa1dea64/20260404_13h22m28s_grim.png)

# Third journal

My schematic was sort of a mess I spent 20 minutes just changing the pinout of the schematic and cleaning it up. A lot of text was overlapping and wires, that said it is not perfect now but its a lot more readable because I changed the pinout and other bits.I dont think I can remove all overlapping wires however I did try to minimise the amount of overlaps. The R5 and 47k text was colliding with the wire so I decided to swap pin 7 and 3!

I also swapped a couple pins in u1 and kept pin 4 near pin 8 because they both connected!I also moved pin 2 to make it a lot more readable and it was closer to the pin 6 wire so it doesnt overlap at all. Note: I didnt swap them on the physical chip or change the footprint or reassign anything I just moved the pins on the schematic editor.

![Image](https://cdn.hackclub.com/019d5d59-4d4e-79ee-b5e9-cf42f8cd5d77/20260405_11h18m33s_grim.png)


