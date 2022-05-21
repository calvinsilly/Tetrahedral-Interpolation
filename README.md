# Tetrahedral Interpolation
![](Tetrahedral_Interpolation_Example_01.gif)

Color transformations using tetrahedral interpolation, includes both an implemention for the expression node and blinkscript.
I never managed to solve an inverse function for this to round trip back, which is something I came really close to but eventually scrapped. So for now only a simple forward operation.

For folks unfamiliar with Steve Yedlin, ASC:
These implementations are supposed to be replications of the one's Yedlin showcasesd. A video where he willingly showed half of the blinkscript code can be found in the end of this page below (0:14:30). Where I only attemped to reconstruct the missing parts with the help of some math from various papers also linked in the end of the page below, which I then later also translated to the expression node for NC Nuke users. 

TetraAutomater is only the suggestion of what it could be doing, since it was never mentioned. 

I just want to be able to share these for everyone to use. So I don't expect any credit from it!

Video demonstration: https://www.youtube.com/watch?v=8kBkYEiAkIw

NEW: Check out a port made for Fusion by Ember Light https://github.com/EmberLightVFX/Tetrahedral-Interpolation-for-Fusion

## TetraAutomater
![](TetraAutomater/TetraAutomater_Example_01.gif)

As the name suggests, matches the 6 colors automatically, given an input and output. Can also be used for an inverse operation but not recommended. The python library SymPy will be required (found SymPy==1.5 to work correctly, newer versions seem to cause issues due to some change to how the solver works).

Originally written for MATLAB by [Juanjo Salazar](https://www.juanjosalazar.com/), solution was later translated to python by [Ethan Ou](https://github.com/ethan-ou/) and now an explicit algebraic solution was found using Mathematica, which avoids the use of python and for solving the same system of equations *everytime*.

## Papers and Resources
- http://www.yedlin.net/DisplayPrepDemo/DispPrepDemoFollowup.html
- https://www.filmlight.ltd.uk/pdf/whitepapers/FL-TL-TN-0057-SoftwareLib.pdf
- https://blogs.mathworks.com/steve/2006/11/24/tetrahedral-interpolation-for-colorspace-conversion/
- https://www.hpl.hp.com/techreports/98/HPL-98-95.pdf
