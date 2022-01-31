# 3. Computer Aided design

## Research
To design and study the raster and vector files, this time I tried Inkscape for 2D, and Fusion360 for 3D, both of which were totally new to me. It took me around 10 days to get used to their basic functions, during which I regulated my emotion, motivation, as well as the cognitive strategies to learn them. Professional and scary as they may be, they can be unbelievably convenient once knowing the logic and mechanisms of the complexity behind them.

## Gallery + Elaboration

### 1. 2D Raster and Vector: Inkscape

This is the 2nd pencil draft of the wooden bag for the final project.
![](../images/inks0.jpg)

As an amateur, I studied thingiverse.com to get inspirations of the wooden box files with their svg files. 
![](../images/inks1.jpg)
![](../images/inks2.jpg)

I defined the parts that need modifications such as the flat bottom, interlocking designs, holes to allow the handle, and the trapezoid front-upper side. 
![](../images/inks4.jpg)

The measurement is crucial in Inkscape design. I got the parameters including slot width and depth.
![](../images/inks5.jpg)
![](../images/inks6.jpg)
![](../images/inks7.jpg)
![](../images/inks10.jpg)

I used eraser function to weed off the unnecessary parts, then closed the side with a straight line. 
![](../images/inks8.jpg)

For the residuals, I used white rectangular blocks to cover. 
![](../images/inks9.jpg)

After the trial, I could focus more on the technical parts for the coming laser cutting: the round corners, the bendable top, etc. So, I used the 3rd pencil draft to help illustrate.
![](../images/inks11.jpg)

After the modification, I still need to change the line width to 0.02 mm for laser cutting, redesign the trapezoid lines, justify the jigsaw teeth interlocking designs, and take kerf into consideration. 
![](../images/inks12.jpg)


### 2. 3D Raster and Vector: Fusion360 

I met some problems using Fusion360 during the week mostly because I felt hesitant and scared of new software. I was anxious about the functions or unfamiliar keyboard combinations of Fusion360, just like when I started to programme at CMD, or Inkscape, or generally speaking, anything new including some classic RPGs such as Neverwinter Night, the Elder Scroll, etc. or living in a new country. It is more about personality. So, I tried to dodge Fusion360, but when it came to Behnaz's week for computer-controlled cutting, I must face it as Inkscape is smart except for one thing: parametric design!
  Therefore, I returned to this week's task then located the function of learning Fusion360 as to understand and try parametric designs. After hours of nervous attempt, I practised designing a pentagon with slots. Since this assignment was completed after week 4's content, I had already got the knowledge of kerf, so would directly post the portfolio here.

First, I randomly drew a pentagon under the menu of sketch + create.
![](../images/fp1.jpg)

Now comes to the parametric design, which Neil, Yrjo, Behnaz as well as numerous vtubers emphasized. The logic is rather simple: Instead of setting parameters by hand for endless times in complicated design, you can just name certain parameters with their expressions (length, angle, etc.). So next time if you change something, click the part + sketch (the radial menu reminds me of the counterpart in Neverwinter Nights). It was chunky at first, but useful after getting used to it. Also, parametric design is powerful as when you constrain certain sides, lengths, angles, and other key parameters, when you change other factors, or feel free to reshape the original design, everything will be automatically and smartly reset which excatly thanks to the parametric restrictions.
![](../images/nwnradialmenu.jpg)

For example, for the pendagon, I named each side as "side". Because in the coming assignment I needed to test laser cutting, I also named a kerf (measured as 0.1mm), the material thickness in 3mm (MDF board), a slot width to be 2.9 mm (=MDF thickness 3mm - 0.1 kerf width). 
![](../images/fp2.jpg)

(After presentation) Behnaz informed me that parametric design was more about using mathmatic equations to define the parameters, which made me refine the work by changing the slotwidth's expression from typing 2.9mm to "mdfthickness-kerf", instantly I noticed that the value was calculated as 2.9mm. I then changed the expression of "halfside" into "(side-slothwidth)/2" to automatically get 25.05mm in value.  
![](../images/fp16.jpg)
 
(After presentation) As a test, I modified the kerf into 0.3mm, then the other related parameters were immediately reset. 
Now, I understand the logic of parametric design: the name is a label for some parameters (length, angle, etc.); the unit is a measurable unit such as mm, degree, etc. in accordance with the parametric nature; the expression is either a typed number, or mathmatic equation to make related parameters interdepend; the value is the "will be input" value shown on the draft. 
![](../images/fp17.jpg)

(After presentation) It worked! the "slotwidth" is still 2.9mm, but defined by equations; The "halfside" was also smartly reset:)
![](../images/fp18.jpg)

To test the convnience of parametric design, I clicked the sketch function of a pendagon side, directly typed the label "side" instead of a number to change it into 72 mm (originally it was 72.654mm).
![](../images/fp3.jpg)

Now I immediately got a modified shape with all 5 sizes changed and interconstraint.
![](../images/fp4.jpg)

Similarly, I drew a rectangle for the slot. Rather than typing numbers, I directly used the parameter names slotdepth (5mm) and slotwidth (2.9mm) to fast set the numbers.
![](../images/fp5.jpg)
![](../images/fp6.jpg)

Indeed, it is quite challenging for an absolute beginner like me to memorize the key steps. Thus, I made a brief note of what I often used after watching videos and clicking around. Sketch allows basic line sketches. You can find basic shapes and lines in create column. The modify functions are easy to use. If it is just a 2D design, the curve corner, scissors, offset can help easily make joint shapes.
For example, in my draft, I made a rectangular slot. If I didn't need the overlapping side, the scissors function can delete the extra side. Constraints have smart but powerful functions to align shapes. In my case, I intended to make the longer side of slot perpendicular to the pentagonal side. I just tried the function with 2 trials. If you move the mouse to each icon, there is a brief description to help understand each constraint logic. 
![](../images/fp8.jpg)

The slot, which consisted of 3 straight lines, can be duplicated so I quickly got 5 same slots for each pentagonal side. The problem arose: How to make the slot perfectly central to each side?
![](../images/fp9.jpg)

Parametric design worked again. To make the practice easier to calculate, I changed the side expression from 72mm to 53mm, allowing 3mm slotwidth (2.9mm in reality due to the kerf). In this way, there was 25 cm for each side if I centered the slot. I set a new parameter named "halfside" to be 25 mm.
![](../images/fp11.jpg)

After repeating the sketch, the use of halfside parameter, I got satisfactory pendagon with slots by simply several clicks.
![](../images/fp10.jpg)
![](../images/fp12.jpg)

All in all, Fusion360 is a powerful and free software to do parametric design. You can see that the parameters are marked in a clear, concise, and professional way. Of course, you can hide the sublines by clicking the eye icon on the left, leaving only the final work you need. 

