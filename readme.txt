Arduino IDE is a simple GUI software that helps the noob guy to interface himself with Arduino environment and ATmega and ATtiny MCU's. What Gioblu Robotics wants to do is simply to broaden the Arduino community by giving noobs the possibility to use many ATtiny and ATmega family MCU's, and to the skilled ones a place where they can put their stuff they want to share with the community. While browsing the web I found many ports of Arduino, so many, in fact, that showing them in the drop down menu is a problem by itself. I am thinking about dividing ATmega and ATtiny families, or some other categorization to reduce the menu's length. 

ISSUES:
- Add a theme button where you can choose a template for your editor
- New fancy icons :P
- "Board" dropdown list modification / split to avoid out of screen list problem
- Add new libraries
- Add new http://www.gioblu.com tutorials related examples 

HOW TO COMPILE THE IDE FROM JAVA FILES

On Linux, you need the Sun Java SDK, avr-gcc, avr-g++, avr-libc, make, ant, and git.

2. Grab the code from GitHub
this grabs the code as an anonymous user.

# grab the code, it'll take a while
git clone git://github.com/gioblu/ArduOpen.git
# (maybe even a long while for you dialup and international folks)
3. Build It
Use the command line.

cd /path/to/arduino/build
ant

# if everything went well, you'll have no errors. (feel free to make
# suggestions for things to include here for common problems)

# then to run it
ant run

# each time you make a change, use ant to build the thing 
# and run to get it up and running. 
Updating to the Latest Version
Each time you want to update to latest version from svn:

cd /path/to/arduino
git pull
git update
If new folders have been added, or you're gettin odd errors, use:

ant clean
