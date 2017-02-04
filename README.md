**CPEN 475/575  - Project 1\_Slots**

**Deliverables:**

Please clean your Android Studio project and then zip the containing directory.  Please work individually on this assignment.

**Target SDKs**

I will compile and test it on a Nexus 5 running some version of Android between API 14 and API 21.

**Provided stuff:**

An apk to demo the program.  An apk is like an executable zip file.  Open it in your email on your device and you should be able to install it.  I&#39;ve tested it on API 23, API 21 and API 19.   I&#39;ve also included a lot of drawables and a file which contains project constants.

**Description**

You are to generate a slot machine app display application.  Once started the user will be presented with a GUI similar to the following;

Figure 1

When started it looks similar to figure 1.  It costs a dollar every time the user clicks the green Go button. When the user presses Go button, all flowers will spin around and then stop. When they stop they will be randomly reset to 1 of 3 colors.  If they match the user earns dollars (see above instructions)

As soon as the user presses Go a reset button will appear in the lower right corner as in figure 2. Pressing this button will reset the game to figure 1.



Figure 2

Notice that the amount of money the user has goes up or down according to the number of times the Go button pressed and winnings.  If the user runs out of money.  The Go button should disappear and the user must hit the reset button to start over.  See Figure 3 for what this looks like.

Figure 3



**Project icon**

Is named top.png Should go in drawable folder, set it in the manifest.

**Info**

The flowers you see above are .png files that go in the drawable folder F1,f2,f3.  They have been made transparent so that you can see through part of them.

The temp flower that all three flowers turn into before they are animated is tmp.png.   When the animation is over each flower is assigned a random color.

The Gold coin(dol.png), Reset(reset1.png) and Go (go.png) buttons are all Imageviews.  The gold coin is not clickable, the others are (android:doClick handler in XML is the easiest).

The background (flowers3.png)  is set in the parent relativelayout using the following

:

**android**** :background= ****&quot;@drawable/flowers3&quot;**
**android**** :scaleType= ****&quot;fitXY&quot;**

:



**How can I make transparent Icons?**

I used [http://www191.lunapic.com/editor/](http://www191.lunapic.com/editor/) Upload a file, Edit-&gt;Transparent.  Choose a transparent color by clicking on it and then save it locally as a png file.

**What about strings?**

Please pull them all from strings.xml in the values folder.

**What about Colors?**

Please pull them all from a colors.xml in the values folder.

**What layouts do I use?**

The layout will likely be the hardest part of this project.  I used a combination of linear and relative layouts.

**Do I have to handle rotations?**

No,

**Grading**

Layout is correct

Flowers animated correctly

Transparent icons correct

Go and Reset work properly

Money is tracked properly

Application icon is set
