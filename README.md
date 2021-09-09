# NGS2-Spawn-Mod-HP-Reduction-Alpha-Story-Chapter-Challenge
# UPDATE 2021-09-09 - Chapter 2 Support Added
# Hotkey removed

THIS MOD WAS ONLY CREATED WITH MASTER NINJA MODE IN MIND, LOWER DIFFICULTIES ARE SUPPORTED FOR ENEMY COUNT INCREASE BUT ENEMY ENCOUNTER TYPES WILL NOT BE MODIFIED. 

IF THE DEFAULT SPAWN AND ENCOUNTER SETUP IS TOO TOUGH, READ THE BELOW ON HOW TO MODIFY SPAWN NUMBERS & ENEMY TYPE

INSTRUCTIONS

1. Download Cheat Engine 7.3

2. COPY & PASTE THE CONTENTS OF NGS2SPAWNMODV02.CT IN NOTEPAD AND SAVE IT AS NGS2SPAWNMODV0.2CT

2. Launch Ninja Gaiden Sigma 2 WITH CHEAT ENGINE

3. ATTACH CHEAT ENGINE TO NINJA GAIDEN SIGMA2.EXE (GAME HAS TO BE LAUNCHED FIRST)

NOTE: ONLY ENABLE THE SPAWN AND ENEMY ENCOUNTER BASED ON THE CHAPTER YOU'RE PLAY AND DISABLE ALL THE OTHERS. THE GAME MIGHT CRASH/SOFTLOCK OTHERWISE


HOW TO EDIT ENEMY TYPES AND ENEMY SPAWN AMOUNT

ADJUSTING SPAWN AMOUNT

Open "Chapter # Increase Spawn"

Option 1: Comment out using // reset values from LINES 29-69

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
Open the file "Chapter # Modify Enemy Encounters"

Adjust the values in setspawn (initial spawn)
   
   mov [greycounter],4
   
   mov [iscounter],8
   
   mov [magecounter],6
 
Adjust the values under: 

resetgreycounter:

resetiscounter:

resetmagecounter:

IM NOT VERY GOOD AT ASM SO HOPEFULLY SOMEONE CAN FIND A BETTER/EASIER WAY TO DO THIS
