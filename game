import random
import time
import os

def clear():
    os.system('clear')

#variables
look = True
hidingPlace = random.randint(1, 8)
start = False
inspect = False
wall = False
sword = False
hand = False

#Hiding places
lamp = 1
topDresser = 2
pillow = 3
closet = 4
chair = 5
rug = 6
middleDresser = 7
bedSheet = 8


#Introduction
print ("You wake up and find yourself alone in a dark room inside a castle tower.")
print ("Glancing around, you realize you are in a bedroom and that you are a prisoner")
print ("You find an unlit torch hanging on the wall and take it down.")
print ("It's too dark to find your way out and escape. You need to find matches!")
print()

#Pre Game
while (not start):
    print ("What is your name?")
    name = input()
    print ("Type \"begin\" when you are ready to start, " + name)
    choice = input().upper()
    if choice == "BEGIN":
        start = True
    else:
        print("Not ready yet "+ name +"?")
        print()

#Game Start
start = time.time()
print ("To see a list of possible commands, type \"help\" at any time")
print()
print ("What do you want to do, "+name+"?")
print()
#print (hidingPlace)

while(look):
    choice = input().upper()
    
#Inspections
    if choice == "INSPECT ROOM":
        print ("There is a lamp, dresser, bed, closet, chair, and rug.")
        print()
    elif choice == "INSPECT LAMP":
        print ("It's an ordinary lamp. Ugly, but ordinary")
        print()
    elif choice == "INSPECT DRESSER":
        print ("It has three drawers and unicorns carved into the side.")
        print()
    elif choice == "INSPECT CLOSET":
        print ("It's a closet, dude.")
        print()
    elif choice == "INSPECT CHAIR":
        print ("It looks comfy...maybe rest for a while?")
        print()
    elif choice == "INSPECT BED":
        print ("It's a bed with a sheet and a pillow.")
        print()
    elif choice == "INSPECT RUG":
        print ("It's a large floor rug.")
        print()

#Lamp Search
    elif choice == "LOOK IN LAMP":
        print ("You can't really look \"in\" a lamp. Try a different command.")
        print()
    elif choice == "LOOK ON LAMP":
        print ("Just a lampshade")
        print()
    elif choice == "LOOK UNDER LAMP":
        if hidingPlace == 1:
            look = False
        else:
            print ("Nothing under there...")
            print()
    elif choice == "LOOK BEHIND LAMP":
        print ("Just a wall with a gross stain back there.")
        print()
        
#Dresser Search
    elif choice == "LOOK IN DRESSER":
        print ("Which drawer? Top, middle, or bottom")
        choice = input().upper()
        if choice == "TOP":
            if hidingPlace == 2:
                look = False
            else:
                print ("It's empty")
                print()
        elif choice == "MIDDLE":
            print ("Its a stuck, but it feels like you can open it if you pull hard... what do you want to do?")
            choice = input().upper()
            if choice == "PULL HARD" or choice == "PULL HARDER" or choice == "PULL":
                print()
                print ("CRAAAACK!!!!")
                print()
                print ("Well, its open, but you broke it. Great job. Do you want to look in the broken drawer?")
                choice = input().upper()
                if choice == "YES":
                    if hidingPlace == 7:
                        look = False
                    else:
                        print ("Nothing in there...")
                        print()
                elif choice == "NO":
                    print ("Quitter...")
                    print()
                else:
                    print ("I don't understand...")
                    print()
            else:
                print ("Giving up already?")
                print()
        elif choice == "BOTTOM":
            print ("There is a sword and shield in there.")
            sword = True
            print()
        else:
            print ("I don't understand...")
            print()
    elif choice == "LOOK ON DRESSER":
        print ("There is a trophy for first place in winning, but it is bolted down. Nothing else.")
        print()
    elif choice == "LOOK UNDER DRESSER":
        hand = True
        print ("Just dust. And somebody's hand.")
        print()
    elif hand and choice == "SHAKE HAND":
        print ("That's gross")
        print()
    elif choice == "LOOK BEHIND DRESSER":
        print("Its snug against the wall, there is nothing behind there")
        print()
    elif sword and choice == "TAKE SWORD" or choice == "TAKE SHIELD" or choice =="TAKE" or choice == "TAKE LAMP" or choice == "TAKE PILLOW" or choice == "TAKE CAT" or choice == "PICK UP SWORD":
        print ("You are already bad at finding matches.  Don't add thief to your list of inadequacies")
        print()
    elif sword and choice == "USE SWORD":
        print ("Why must you always resort to violence? Just find the matches...")
        print()
    elif choice == "PULL DRESSER":
        wall = True
        print("You moved the dresser and exposed the wall")
        print()
    elif wall and choice == "INSPECT WALL" or choice == "LOOK ON WALL" or choice == "LOOK WALL":
        print("It looks like something is written there..")
        inspect = True
    elif wall and inspect and choice == "READ WALL" or choice == "READ WRITING" or choice == "READ":
        print("_________                        __             .___ ___.")           
        print("\_   ___ \_______   ____ _____ _/  |_  ____   __| _/ \_ |__ ___.__.") 
        print("/    \  \/\_  __ \_/ __ \\\__  \\\   __\\/ __ \\ / __ |   | __ <   |  |") 
        print("\     \____|  | \/\  ___/ / __ \|  | \  ___// /_/ |   | \_\ \___  |") 
        print(" \______  /|__|    \___  >____  /__|  \___  >____ |   |___  / ____|") 
        print("       \/              \/     \/          \/     \/       \/\/     ") 
        print("          ____.  ")                                           
        print("         |    | ____   ____   ____   ______")                 
        print("         |    |/  _ \ /    \_/ __ \ /  ___/")                 
        print("     /\__|    (  <_> )   |  \  ___/ \___ \ ")                 
        print("     \________|\____/|___|  /\___  >____  >")                 
        print("                          \/     \/     \/ ")   
        print()
    elif wall and inspect and choice == "ERASE" or choice == "WIPE OFF" or choice == "ERASE WALL":
        print("How dare you")
        
#Bed Search
    elif choice == "LOOK IN BED":
        print ("Do you mean \"Look under sheet\"? Maybe that would reveal something...")
        print()
    elif choice == "LOOK ON BED":
        print("A sheet and a pillow. Trying searching around those")
        print()
    elif choice == "LOOK UNDER BED":
        print ("Nothing under there but some skeleton... maybe he couldn't find the matches either.")
        print()
    elif choice == "LOOK BEHIND BED":
        print ("A wall")
        print()
    elif choice == "LOOK UNDER PILLOW":
        if hidingPlace == 3:
            look = False
        else:
            print ("Just somebody's tooth. Maybe it's waiting for the toothfairy?")
            print()
    elif choice == "LOOK UNDER SHEET":
        if hidingPlace == 8:
            look = False
        else:
            print("      |\      _,,,---,,_")
            print("ZZZzz /,`.-'`'    -.  ;-;;,_")
            print("     |,4-  ) )-,_. ,\ (  `'-'")
            print("    '---''(_/--'  `-'\_)  ")
            print ("Just a cat sleeping under there. Maybe try petting the cat?")
            print()
    elif choice == "LOOK BEHIND PILLOW" or choice == "LOOK IN PILLOW" or choice == "LOOK ON PILLOW" or choice == "LOOK BEHIND SHEET" or choice == "LOOK ON SHEET" or choice == "LOOK IN SHEET":
        print ("Not really a good option. Try looking a different way.")
    elif choice == "PET CAT" or choice == "PET" or choice == "PET THE CAT":
        print ("OUCH! That's a nasty bite. Better leave the cat alone...")
        print()

#Closet Search
    elif choice == "LOOK IN CLOSET":
        if hidingPlace == 4:
            look = False
        else:
            print ("Just a lot of old clothes...")
            print()
    elif choice == "LOOK ON CLOSET" or choice == "LOOK BEHIND CLOSET" or choice == "LOOK UNDER CLOSET":
        print ("Logically speaking, the only thing you can really do is look \"in\" a closet.")
        print()
            
#Chair Search
    elif choice == "LOOK IN CHAIR":
        print ("You want to cut it open and look inside the chair? I promise it is only stuffing. Let's not destroy more than we have to.")
        print()
    elif choice == "LOOK ON CHAIR":
        print("Nothing on the chair but some comfy cushions. Maybe sit? Or look underneath?")
        print()
    elif choice == "LOOK UNDER CHAIR":
        if hidingPlace == 5:
            look = False
        else:
            print ("Just empty space. Looks like a good place to store boardgames.")
            print()
    elif choice == "LOOK BEHIND CHAIR":
        print ("It's a wall.")
        print()
    elif choice == "REST IN CHAIR" or choice == "REST ON CHAIR" or choice == "REST" or choice == "SIT IN CHAIR" or choice == "SIT ON CHAIR" or choice == "SLEEP" or choice == "NAP":
        print ("Ain't nobody got time for that! Find those matches!")
        print()
            
#Rug Search
    elif choice == "LOOK ON RUG":
        print ("It wouldn't be much of a hiding place if it was sitting on top of the rug, now would it?")
        print()
    elif choice == "LOOK IN RUG":
        print("Um, its a rug.  You can't keep things inside a rug. You can keep things on top or under.")
    elif choice == "LOOK UNDER RUG":
        if hidingPlace == 6:
            look = False
        else:
            print ("Nothing under there...")
            print()
    elif choice == "LOOK BEHIND RUG":
        print ("Say that outloud to yourself. Does it make any sense?")
        print()
            
#Other Commands
    elif choice == "QUIT" or choice == "STOP":
        print ("Yeah, you can't actually do that. You need those matches or you...well, have you looked under the bed?")
        print()
    elif choice == "HELP":
        print ("Try using the command \"inspect\" followed by an item in the room.")
        print ("If you don't know what is in the room, try typing \"inspect room\".")
        print ("To look for the object in the room, try typing \"look\" then a prepositon followed by the item.")
        print ("Prepositions you can use: in, on, under, or behind")  
        print ("For example, typing \"look under bed\".")
        print()
    elif choice == "CLEAR":
        clear()
    else:
        print ("I do not understand...maybe try a different preposition or command?")
        print()
        
#End Game
end = time.time()
print ()
print()
print ("You found it! Good work, " + name + "!")
print()
print()
print ("           /|")
print ("        /\\/ |/\\")
print ("        \\  ^   | /\\  /\\")
print ("  (\\/\\  / ^   /\\/  )/^ )")
print ("  \\  \\/^ /\\       ^  /")
print ("    )^       ^ \\     (")
print ("   (   ^   ^      ^\\  )")
print ("    \___\\/____/______/")
print ("    [________________]")
print ("     |              |")
print ("     |     //\\\\     |")
print ("     |    <<()>>    |")
print ("     |     \\\\//     |")
print ("      \____________/")
print ("          |    |")
print ("          |    |")
print ("          |    |")
print ("          |    |")
print ("          |    |")
print ("          |    |")
print ("          |    |")
print()
print()
print("It only took " + str(round(end - start,2)) + " seconds to find it, "+ name +".")
