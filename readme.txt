Star Trek Bridge Crew Repair Hull Instructions

1. Open Assembly-CSharp.dll, in the game directory, in dnSpy (I used dnSpy v6.6.0 (64-bit, .NET)

2. Open UnityEngine.UI.Text

3. Add the code found in RepairHullCode.Text.UI.txt file. I added it after the code for "public virtual int layoutPriority".  Do not paste the code in that function.  Paste the code after that function. 

4. Open 'Sector.Spacecraft.Subsystems.HullServer  and look for BatchUpdate().  

5. Add the line 'Text.CheckStationRepair(this);' to the function to call the CheckStationRepair function.  

6. Right click in the BatchUpdate() function and go to 'Edit IL Instructions'.  

7. Look at the image for 'Edit IL Instructions' and make yours look the same. You have to click on things and use the drop down list. 

8. File->Save Module

9. Try it out.  The dlls are available here if you want them:  https://www.nexusmods.com/startrekbridgecrew/mods/7 



  