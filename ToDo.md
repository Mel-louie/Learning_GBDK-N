# To do on standby (forever)]

:radio_button: to do; :ballot_box_with_check: OK; :exclamation: priority; :scissors: not a thing anymore<br><br><br>

:radio_button: update the readme's gif<br>
:radio_button: adding sound<br>

:radio_button: exterior with a scroll (! the player moves with the screen limits)<br>

:ballot_box_with_check: collision with png<br>
:ballot_box_with_check: animate png<br>
:ballot_box_with_check: add a cat<br>
:ballot_box_with_check: add a roomate<br>
:ballot_box_with_check: to fix: bug intercat when moving<br>
:ballot_box_with_check: refacto with struct for the sprites<br>
:ballot_box_with_check: hide the sprite when window + sprite at the bottom of the screen<br>
:ballot_box_with_check: interact with all the background<br>
:scissors: recreate tilesets (i'll do that for a real game)<br>
:ballot_box_with_check: create sprites for cat and roomate<br>
:ballot_box_with_check: interact without walk...<br>
:ballot_box_with_check: correct player animation when colision, should move in the right direction<br>
:ballot_box_with_check: clean the title screen and found the dot bug<br>
:ballot_box_with_check: change player colors<br>
:ballot_box_with_check: add a title screen with a press start button to enter the game<br>
:ballot_box_with_check: splash screen with fadding palette<br>
:ballot_box_with_check: manage collisions with background<br>
:ballot_box_with_check: tidy up the files + comments<br>
:ballot_box_with_check: create and animate a real sprite <br>
:ballot_box_with_check: pimper les Makefile<br><br><br>

<h3>:green_book:random notes</h3>
To have the right shades of color for a sprite (black, gray, white, and light gray transparent):<br>
	- draw with WHITE for transparence, and LIGHT GREY for white;<br>
	- convert to gb with img2gb ans this commande:<br>
	img2gb tileset \<br>
    --output-c-file=../src/tiles_player.c \<br>
    --output-header-file=../includes/tiles_player.h \<br>
    --output-image=./player.sprites.png \<br>
    --sprite8x16 \<br>
    --name PLAYER_SPRITES1 \<br>
    ./player1.png<br>
	- when init sprite, add this change fot default palettes: 'OBP0_REG = OBP1_REG = 0xe2';<br>
	- can test other combinason<br><br>

memo palette:
put the hexa values avoid to have 'warning 158: overflow in implicit constant conversion' which is not great

b 11
g 10
l 01
w 00

PALETTE(WHITE, LIGHTGR, GREY, BLACK) = 11100100 = 0xe4
PALETTE(LIGHTGR, GREY, BLACK, BLACK) = 11111001 = 0xf9
PALETTE(GREY, BLACK, BLACK, BLACK) = 11111110 = 0xfe
PALETTE(BLACK, BLACK, BLACK, BLACK) = 11111111 = 0xff

memo text:

19 char/line
