# 4. Computer controlled cutting

This week Behnaz taught us how to use vinyl cutter and laser cutter. To get a svg file, the simplest way is to practise using Inkscape. This time, I had to force myself to use Fusion 360 to do parametric design before transfering it to an svg file. Fusion 360 is inescapable as Inkscape is powerful only except for parametric design. 


## Research
First key notion to keep in mind:  

- raster-for engraving, which is about dots, pixels;  

- vector-for cutting, which is about lines, flames (as more beam power is focused).  


The toughest part was the usage of fusion360.  

At first, I was afraid of the new, professional software but with the encouragement from Antti, Diep, and Behnaz, I calmed down, watched Neil's intro video, youtube tutorials, and some Chinese geeks' clips.  

After a good sleep, I opened fusion360, randomly drew a pentagon, tried some constraints, clicked here and there to explore the parameter setting window before it accidentally worked!  

The same feeling took place again, which was just like those for Github programming as well as Inkscape. I could literally feel the convenience of parametric design and the reason to use it over Inkscape.  

Mentally, it proved learning curve again:  
- Inkscape-5 days;  
- Github very basic programming-12 days;  
- Fusion360-7 days.

## Gallery + Elaboration
### 1. vinyl cutting
### observation and practice 
Starting from a basic Inkscape pattern, it is a good habit to add a frame for the convenience of later weeding. Weeding, according to Neil's video, means peeling the unnecessary parts. Ctrl + Shift + R can allow me to resize page to drawing or selection in Document Properties. 
![](../images/vp1.jpg)

To open or close the Roland vinyl cutter, push the handle at the left back side. Then, the two wheels can be lifted.
![](../images/vp2.1.jpg)

It is a must to place the vinyl paper between the two wheels. The wheels must also be within the white label ranges in order to be detectable by the machine.
![](../images/vp2.2.jpg)

If you want to get a more precise measurement of the vinyl paper, you can press preference in printing window, then click "Get from Machine". This allows the scanner of the vinyl cutter to horizontally run across the vinyl paper. 
![](../images/vp3.jpg)

To transfer the svg file to Roland vinyl cutter, find Roland CutStudio in Extensions, then press "Open".
![](../images/vp4.jpg)
![](../images/vp5.jpg)

It is advisable to select "Edge" in Sheet category. 
![](../images/vp6.jpg)

Here we go. A note: the size of the vinyl paper should be moderate. Avoid thin one. Importantly, the most obvious difference between vinyl and laser cutter is that vinyl cutter literally uses sharp knife to press on the material to get the lines.
![](../images/vp7.jpg)
![](../images/vp8.jpg)

The most standarized way to weed (peel) the usable sticker is to use tweezer, especially when there are exquisite spots or lines. Of course, if they were just basic patterns, or to make the lessons more attractive to youngsters, fingers and hands are parallelly flexible tools. 
![](../images/vp9.jpg)

Transferring sheets are powerful if you want to save the cut work for later use. The tough side of vinyl paper is slippery, allowing transferring sheet to attach them tightly. After this procedure, you can get both the stikers and transferring sheets to show the sticky sides. Be careful of the dusts, of course.
![](../images/vp10.jpg)

The end of observation and practice session. Quite straightforward experience. The frame is an important part to allow convenient weeding. Also, it helps to justify positive and negative patterns as later I encountered when doing my own giant panda printing practice.
![](../images/vp11.jpg)

### self design and final work

Below is the panda file I used for vinyl cut. I used Inscape and Extention-Roland CutStudio to finish the software part.  

[The svg file for the panda](../files/panda.svg)  


Without much talk, I got a panda bear svg file from the Internet, added a frame in Inkscape, exported it to Roland Cutstudio, made 3 sizes, then set up the cutter (mode: edge) as in the observation session.
![](../images/vd1.jpg)

I used black vinyl as panda bear fur is a combination of white and black. 
![](../images/vd2.jpg)

When it came to weeding (peeling), Diep asked about how to define which parts to leave. To be honest, I had the same concern the day before. My friend who knows seal cutting comforted me that it is my justification of positive and negative effects. Therefore, you can see that on the left side, the little pattern was the residual that I didnt need simply because I knew the color distribution of panda. Also, as you can see, the larger the sticker is (mine largest size was 70mm), the easier to weed and to allow more complicated line designs.
![](../images/vd3.jpg)

After weeding, I got the stickers I needed. How to transfer them? Transfering sheet was helpful. Press it hard to the work, lift then get the usable stickers. Be careful since the panda show their skicky sides to me.
![](../images/vd4.jpg)

The final work looks great. The sticky side was quite strong. Also, the rough side seems durable.
![](../images/vd5.jpg)

***
***
***

###2. laser cutting

### observation and practice 

No matter how beautiful the design is, to get the laser cutting started, Behnaz showed us the safety issues that everyone should be serious about: 

1. NEVER LET THE LASER CUTTING WORK ALONE. ALWAYS KEEP AN EYE ON IT. Luckily, FabLab Oulu installed a separate sensor to detect whether there are people within 2 meters when the laser cutting is on. 
2. To turn on the laser printer: turn the round pääkytkin (headswitch) from 0 to 1 → turn the red handle to the air inside of the cutter flow (it is crucial as the air can circulate within the printer and clear off the combustion residuals which are hazardous). → Turn on the power switch of the machine. 
![](../images/lcp1.jpg)
![](../images/lcp2.jpg)
![](../images/lcp3.jpg)
3. If something really starts to ignite, number one: stay calm. Number two, open the laster cutter lid to activate the interlock. However, if you are materials like cardboard gets more flames because of the input air, rush to get the nearby FabLab fire blanket to smother the fire. Fire blanket should be the first priority as extinguisher is ok but it may create a huge mess to the machine (maybe cost even more to repair afterwards :(), never to say not many people know how to properly use the extinguisher. A fire blanket looks like below:
![](../images/lcp14.jpg)

Behnaz first introduced us a key concept of laser cutting that is directly related to parametric design: **kerf**.  
Kerf is the part that laser beam burns away, which is why laser can "cut" materials. When we do parametric design with consideration of high precision, **the width of kerf** matters.  
  - For example, I hope to set the pentagon slot width to be 3mm. If I set the number to be 3mm, the kerf will make it more than 3mm, which can cause instability when interlocking the slots. That was the reason I set the parameter of "slotwidth" to be "material thickness - kerf", instead of assigning a fixed number.  
  
  But what is the width of **kerf**? Behnaz asked us to laser cut on our own to see if there are kerf differences among materials.
![](../images/lcp4.jpg)

It is rather easy to laser cut. There are two steps:  

1. **Desktop**. Open svg file in Inkscape → set the line width to be 0.02 mm → save as PDF file → open the PDF file → ctrl + p → examine the Advanced and General windows to set up the printing parameters. → press save and ok  
   
First, save the Inkscape svg file as PDF file. Open the pdf, click the printing to get the blue window → Click the Advanced option to choose the preset modes (i.e., In our session, we used 3mm-MDF-engrave+cut and 3mm-acrylic-engrave+cut) → Finalize the setting in General opion. 300 DPI is fair enough for most cases; raster is for engraving while vector is for line cutting; The speed, power and frequency are the independent variables to control the laser beam results. The beam power is stronger either with slower speed, more power or frequency.
![](../images/lcp5.jpg)

We also learned the meaning of DPI. It stands for "dots per inch". As each time the laser beam burns a little "dot" of the surface, when the dpi is 254, the laser beam can surely burn every corner of the inch. In this regard, the preset dpi 300 assumes that there are overlapping burnt parts, which is enough for most engraving work. Otherwise, the surface might be over engraving (burnt like chocolate). 
![](../images/lcp6.jpg) 

2. **Laser Cutter**  Open the lid →  place the cutting material on the working table → set the Focus/Jog → select the Job → Press go → MONITOR THE CUTTING PROCESS AND DON'T GO AWAY FOR SAFETY REASONS.  

First, open the lid, place the cutting material on the "bed", or working table. Press it with metal weight if necessary.  

Then, to run the laser cutter, look at the small screen. Use the joystick to move up and down to select the functions. Do three things in a row:  

   1. **Set Focus**. Laser beams are generated, output, then concentrated at the "waist" point where the power is the strongest. The reason to set the focus is hence to get the "beam waist". Since the laser producer tool's height is fixed, you should move the "bed", or the working table up and down to realize the focus setting.  
                 - Use a triangular plate to hang between the two screws of the laser cutting head. The hight of the plate is , so we can assume the beam waist is at the acute angle of the triangle.  
				 - Turn the joystick left to select the speed. Two arrows means fast, one arrow means slow. Usually you will start from the fast mode. Then turn the joystick up and down to move the working table. When you feel the triangle touches the material, shift it to slow mode to adjust the focus gently.  

				 
   2. **Set Jog**  
   
   3. **Select the Job** 

Diep and Antti R measured the MDF kerf (around 0.1mm). Another Antti and me measured acrylic kerf. I used the vernier caliper twice. The first result was 0.065 mm, which was biased because I hadn't put the 10 small chips tightly together. When I did it twice, the result was more reasonable: 0.102 mm. In this regard, I could estimate that the kerf for acrylic laser was 0.1mm and set it in the parametric design.
![](../images/lc6.jpg)

Then, we tested different laser speed and power on MDF to see different effects. 
![](../images/lcp7.jpg)
![](../images/lcp8.jpg)

The results are meaningful: for vector cutting (upper part), the default values worked well, but if the speed was 40 (too fast), the laser could not cut through the MDF. Similar result happened if the power was only half (50%). When the speed is defaulted while removing 20% of the power, the vector cut still went well. We estimated that the vector cut on MDF could be effective if the power is above 60%. The frequency seemed to have little effect on vector cut (middle). The different raster (lower part) settings had remarkable effects on the engraving results. Even on the same surface, you can set different degrees of raster by changing the power. 
![](../images/lcp9.jpg)

We also tested different laser conditions on acrylic. 
![](../images/lcp10.jpg)

The results are interesting: If the speed is 80% with other settings being defaulted, the laser cannot cut through the acrylic. When engraving, if the power is 5, you simply could not see apparent patterns on the surface. We were joking that it might be "useful" in cheating :)
![](../images/lcp11.jpg)
![](../images/lcp12.jpg)

At last, we also tested the different focuses of laser beam. The laser beam was most concentrated on the thinnest point, or the "waist", which has the most power. The upper and lower parts are like a sand clock. The results were not so obvious by appearance, but if I touched the engraved surfaces, the focused one was indeed tougher than others. 
![](../images/lcp13.jpg)


### self design and final work

Below are the files I created and used in actual work. This time I used Fusion360 to design the pentagon, and Inkscape to set up for laser cutting. 

[The f3d file for the pentagon](../files/pentagon_kecheng_f3d.f3d)  
Note: **.f3d** is Fusion 360's native 3D model format.  

[The stl file for the pentagon](../files/pentagon_kecheng_stl.stl)  
Note: **.stl** is the global format to describe the surface geometry of a 3D object.
 
[The pdf file for the pentagon](../files/pentagon_kecheng_pdf.pdf)
Still a note: pdf stands for **portable document format**. 


Thank you Behnaz for helping me understand the meaning of those formats. Also thanks Antti R to help me with the codes for hyperlink in Github. 


In week's three's fusion360 tiral, I drew a pentagon with slots. In this week's laser cutting, I thought things would be quite easy and straightforward with several steps like drawing, printing and analysing. However, I was so naive that the first step of this week was problematic, which ultimately made me refine and reflect on the trouble that I wanted to dodge. In the picture below, I found it a bit strange with unconnected lines.
![](../images/f360eplp1.jpg)

I clicked the drawing view settings and found that the lines were connected if I changed the scale in to 1:2. Then I happily exported it into pdf format.
![](../images/f360eplp2.jpg)

When I inspected the pdf file in Inkscape, I found the problem: ok, everything was shrunk into half size including the slot. Apparently, I could not use a slot with 1.5 mm in MDF.
![](../images/f360eplp3.jpg)

As time was very limited, I needed to hand in some tentative assignments on time, I directly used Inkscape to close the 1:1 scale pentagon lines through drawing.
![](../images/f360eplp4.jpg)

Then, I selected all the lines to set the width to be 0.02 mm for laser cutting (not graving).
![](../images/f360eplp5.jpg)

I observed that the laser cutting work ran twice: first to cut the unconnected lines, then pinpointedly cut the modified parts from Inkscape, which proved its smartness in 2D design. 
![](../images/f360eplp6.jpg)

I duplicated the pentagon to get 5 extra pieces.
![](../images/f360eplp7.jpg)

After waiting for 1 minute, I took out the pieces. Before playiny, I used the vernier caliper to measure the side and slot. The results were satisfactory: side-53mm; slotwidth-0.3mm (0.1mm's credit for kerf).
![](../images/f360eplp8.jpg)
![](../images/f360eplp9.jpg)

Finally I could play the pieces by putting them together. It looked stable and nice.
![](../images/f360eplp10.jpg)

I particularly checked the interlocking part: since the slothdepth was 0.5 mm, the total interlock depth was 1.0 mm. It was fairly stable, but would be better If I made the slotwidth deeper, say, 1 mm. Also, the nodes and other interlocking designs are all worth exploring. 
As for the function, pentagon looks elegant, so I would use Inkscape to draw some patterns or pictures and use it as a badge. The wizard card in Harry Potter is a good example. 
![](../images/hpwc.jpg)

I thought it was over until I showed my concern of the unconnected lines in the drawing. Behnaz explained how the function of extrude works, which opened a great DLC of the week's project and occupied all my free time in 2022 lunar new year, which unexpectedly made me learn something new.

I clicked the pentagon, extruded with 3mm (to match the MDF thickness), got a 3D object, and thought everything was ok. However, the lines were still not connected in the drawing, which drove me confused at night.
![](../images/f360eplp11.jpg)
![](../images/f360eplp12.jpg)
![](../images/f360eplp13.jpg)

I consulted Diep. She calmed me down then helped me through remote screen sharing. She suspected that I hadn't selected the whole shape but only the frame whose extruded version had not covered the whole design. I tried again by drawing and extruding a new pentagon. This time the whole shape was selected.
![](../images/f360eplp14.jpg)

Then, I created a drawing and ok, scale 1:1, lines connected. At least it was clear that the lines could only be closed as long as the object is extruded on a surface rather than the frame.
![](../images/f360eplp15.jpg)

This time I was stuck because no matter how I changed the "select", the pentagon with slots was like a hollow ghost which was too naughty or transparent to be captured. I nearly gave up until I clicked the "surface" and added a "patch" to forcely create a surface within the shape. It seemed successful.
![](../images/f360eplp16.jpg)

As the direction was reversed, I set the extrude parameter to be -3 mm. 
![](../images/f360eplp17.jpg)

It worked in a rather weird way...
![](../images/f360eplp18.jpg)

I didn't care anymore, created a drawing and finally got a proper work even though the procedure was not the optimal. Luckily I don't have the passion to celebrate anything, and this is the most meaningful, diligent and hard working lunar new year so far in my life.
![](../images/f360eplp19.jpg)

