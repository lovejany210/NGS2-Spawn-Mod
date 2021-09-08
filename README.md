# NGS2-Spawn-Mod-HP-Reduction-Alpha (Currently Chapter 1 support) (HP Reduction will work for any chapter)
# Only tested with story mode but apparently it works for Chapter Challenge as well
# I will add support for more levels and keep updating the trainer as I find time

CURRENT SCRIPT WILL ONLY WORK FOR CHAPTER 1 IN STORY MODE ON MASTER NINJA

INSTRUCTIONS
1. Download Cheat Engine 7.3
2. Launch NGS2SpawnMod.CT
3. Attach Cheat Engine To Ninja Gaiden Sigma2.exe

HOTKEYS
1 = Increase Spawn
2 = Modify Enemy Encounters
3 = Reduce Enemy HP Half
4 = Reduce Enemy HP Low
5 = Reduce Enemy HP Very Low 

MY RECOMMENDATION IS TO ENABLE 1,2,3. IF YOU'RE SPAWNING A LOT OF ENEMIES, I WOULD USE OPTION 4 INSTEAD OF 3

HOW TO EDIT ENEMY TYPES AND ENEMY SPAWN AMOUNT

ADJUSTING SPAWN AMOUNT
Open "Chapter 1 Increase Spawn"
Option 1: Comment out using // some reset values from LINES 29-69
Option 2: 77-240 are all the encounters in chapter 1. You have 3 options that you can set each encounter to: 
je startspawnlow
je startspawnmedium
je startspawnhigh
je startspawninsane

Adjust each encounter as needed

Option 3:
startspawnlow
startspawnmedium
startspawnhigh
startspawninsane

Change the value of cmp [counter],(Number).

I.E startspawnmedium is cmp [counter],40 - lower the number to decrease the amount of enemies spawned & increase the number to increase the amount of enemies spawn. I find the values between 25-60 are good

ADJUSTING ENEMIES THAT SPAWN
Open the file "Chapter 1 Modify Enemy

Adjust the values in setspawn (initial spawn)
   mov [greycounter],4
   mov [iscounter],8
   mov [magecounter],6
 
Adjust the values under resetgreycounter,resetiscounter,resetmagecounter
