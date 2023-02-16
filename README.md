# classroom-math-tools
A set of open hardware tools for exploring concepts in math classrooms.

This is a catch-all repository for a series of open hardware tools that I'm developing for use in math classrooms. I've got a few early designs and 
prototypes that I'll be adding to this repository, but these are definitely in the early prototype phase, and aren't ready for actual release or use.
My main goal here is to declare my intentions for the types of products these will be, and the type of open hardware license they'll be released under.
I'm probably going to use the CERN Open Hardware License for this project, and the MIT license for the software. The purpose of this readme is to
declare my intentions in broad terms. The design files for these tools will be freely available for anyone to use, make, and modify, as long as they
attribute to the original project and share them with a similar license. I will also make a small stock of these products and have them available for sale
for anyone who doesn't want to or can't make them themselves. Basically, I'm envisioning this to be a project similar in spirit to Arduino, where
there is an original maker who makes and sells official versions, but other people are perfectly free to make their own versions as well. 

This is a meta-repository. Each project below will have its own repository, to which I will provide a link.

# The math tools I'm developing are as follows:
## A mechanical unit circle demonstrator.
This is a device that uses perpendicular Scotch Yoke linkages to isolate the horizontal and vertical motion of a pin on the end of a crank to show
the sine and cosine components of rotational motion. There are markers on each Scotch yoke that point to values of sine and cosine as the crank rotates,
showing the associated value for each degree of rotation (rotation is shown in both radians and degrees). There are animations that work like this,
but I have given early versions of this to students, and I found that by playing with a physical representation of the unit circle, they immediately 
grasp the relationship of sine and cosine to rotational motion.

I'll be providing the files for 3D printing or laser cutting the parts. I'm on my 5th iteration, which I'll upload here soon, but it's still to complex,
and I'll be simplifying the design in another iteration soon. 

## PCB Slide Rules
The slide rule is an elegant physical computer that I think needs to make a comeback in classroom use. It requires you to build a strong sense of base-10
place notation, and does an excellent job of making arcane concepts like logarithms tangible. In my time teaching math, I've found that kids are incredibly
currently incredibly reliant on access to calculators, or even to just asking Siri what the product of two numbers is, which absolutely blows my mind. 
I think one remedy to this is teaching them to use slide rules to build capability with mental calculation. The slide rule makes mental calculation a tangible,
kinesthetic experience, which helps form stronger conceptual memories. It's also incredibly elegant, and they got us to the moon!

You can only buy slide rules as one-off collectors items these days. The excellent International Slide Rule Museum has classroom loaner sets, but there are only
a few of those, and they are also old and potentially fragile. We need new, durable, inexpensive slide rules, which is why I'm designing them to be manufactured
as PCBs! PCBs are the perfect medium for this. They're cheap, durable, and provide very accurate detailed silk screens or traces that can be used as the scales.
I'm writing Python code that generates SVGs for the scales, which can be turned into PCBs via KiCAD. Anyone will have access to the final PCB files for 
manufacture, and I'll maintain a small stock of them to sell as sets. 

## PCB Vernier Calipers
Accurate measurement is a real challenge in the classroom. I'm working on a design for calipers that use a Vernier scale, and like the slide rule, these will
be made as PCBs. This should make them accurate and inexpensive, democratizing classroom access to precision measurement tools.

## Theodolite / Total station
This is in the incredibly early design stages, but I'm creating a laser cut plywood theodolite. I'm going to use something like an airsoft scope
for the sight, which will provide cheap access to decent optics with crosshairs for precisely targeting objects. Eventually I would like to design my own scope
using lenses so that students can explore concepts of optics. I'm designing Vernier scales for the scales that measure degrees of rotation, and these will be
manufactured as PCBs. Students will be able to use one of these on a tripod to precisely measure distances and elevations using concepts of trigonometry. 
Take the trig class outside for a day of cartography! 

## Triangle Definition Explorer
These are sets of essentiall protractors with long slotted arms on them. You can connect these to each other with special bolts to make triangles. The protractor
parts allow rotation, so you can define the angle of each vertex, and the slot parts allow the joints to slide so that you can define the side length of a triangle.
This allows students to tangibly explore the various methods of rigidly defining a triangle (e.g., Side-Side-Side, Side-Angle-Side, etc.). More of these could
be connected to explore things like 4- and 5-bar linkages. The real innovation here is in the special joining bolt, which allows you to independently lock
isolation and rotation using two different knobs. This makes it so that you can do something like define two vertex angles, lock them in place, and then change the 
length of the side between the vertices to see what effect that has on the overall triangle. The current version of the joining bolt works and is 3D printable,
but is too delicate for release and actual use. I'm working on revision 2, which uses threaded rod and some other changes to be more durable and easier to assemble.

## The Graphing Game
This one is hard to explain, but it's basically an unpowered Cartesian plotter. Each axis will be driven by a timing belt, but the point is that they are driven by 
hand. Kids will be able to use a series of pulleys to link the X and Y axes to each other in different ratios, creating physical representations of linear equations.
There will be paper overlays for the graphing area that show a graph, and the task for students will be to build a system of pulleys that recreates the motion
of the graph. When the slide the x-axis by hand, the y-axis will be driven by the pulleys. So if you want to make the graph y=2x, build a 2:1 ratio pulley system
connecting the axes. I've also got some ideas for how to make add-ons that will enable graphing sine, cosine, tangent, and simple parabolic and exponential functions.
I envision this as a puzzle game in which kids have to figure out how to build a pulley system that will recreate the graph on the overlay, getting progressively
harder over time. I have early designs that use 3D printed parts and precision ground steel rod as linear rails, but there's currently too much friction and racking
in the system to be functional. I plan to experiment with timing belts, and with round polyurethane belts. I'm inclined to use the latter as it's cheap, and 
well-suited to use with 3D printed pulleys.

## Whiteboard Compass
This is a beam compass made for use on whiteboards. Commercially available whiteboard compasses are terrible. The beam compass isn't perfected, but it's already
substantially easier to use than commercial whiteboard compasses. I'll be modifying it to use magnets on the foot in addition to silicone grippers. 
