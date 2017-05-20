# star-trek-game-cmd-beta0.1
@echo off
color f

:speak1enterprise
::enterprise
cls
echo welcome to the enterprise
pause
echo pick an option to witch to speak (1,2,3)
echo 1)its an honor to be here captain picard
echo 2)how did I get here
echo 3)....
pause
set /p speak1enterpriseOption=

if '%speak1enterpriseOption%' == '1' goto picardresponse1
if '%speak1enterpriseOption%' == '2' goto picardresponse2
if '%speak1enterpriseOption%' == '3' goto picardresponse3
:picardresponse1
echo well it wont be if we cant get rid of these romulans
pause
echo (background wharf says) Setting phasers to full power
pause
echo (picard) FIRE!!!
pause
echo romulans are no more
pause
echo good job cadet you survived your first romulan attack
pause
echo now lets talk about your postion
pause
echo you scored top of your class
pause
echo well there is no doubt im making your my new first officer
pause
echo get to quarters number 1
pause
echo (player) number 1?
pause
goto choosename

:picardresponse2
echo you were beamed up from star fleet acadmey at what seem the worst timing to beam a cadet here as they beamed you up these romulans warped here and started to attack us
pause
echo (picard) lt.wharf FIRE when ready.
pause
echo (wharf) phasers ready.
pause
echo (picard) FIRE!!!
pause
echo (romulans are no more.
pause
echo (player) captin I was top of my class in science enginering and tacticality
pause
echo (picard) well you have to choose only one of those. 
echo but instead iam making you my first officer.
pause
goto choosename 

:picardresponse3
echo well then (lt wharf) fire when ready 
pause
echo firing sir
pause
echo well lets see your reports
pause
echo so you were top of your class
pause
echo well were making you my new first officer
pause
goto choosename


:choosename
cls
echo capt.picard: It seems I don't remember your name. What is it?
set /p name=
pause
if '%name%' == '' goto choosename

cls
echo Hi %name%! It's nice seeing you again
pause

:girlorboy
cls
echo %name%, Are you a boy or a girl?
echo (Enter 'boy', or 'girl')
set /p gender=
pause
if '%gender%'=='boy' goto skip
if '%gender%'=='girl' goto skip
goto girlorboy
skip
:skip
echo capt.picard Aah.. so you are a %gender% %name%
pause
goto quarters

:quarters
::quarters1
echo interacting with quarters
pause
echo select an option please
pause
echo 1) talk with the captin
echo 2) sleep (save)
echo 3) make a log (stardates always start with the earth year and ends with .numerical order digit this one will start with 0 then go to 1 then to 2 please follow these as they help star fleet understand what happens and you may enjoy reading these later so want to keep them in order
pause
set /p quartersoption=

if '%quartersoption%' == '1' goto captainResponses1
if '%quartersoption%' == '2' goto save
if '%quartersoption%' == '3' goto logs

:captainResponses1
echo iam busy right now ill see you on the bridge asap
goto bridge

:save
echo this is unopreable and likely never will be
goto bridge

:logs
::logentrymenu
echo would you like to make a log entry
echo 1) yes
echo 2)no 
set /p logentry

if '%logentrymenu%' == '1' goto logentry
if '%logentrymenu%' == '2' goto bridge

:bridge
echo (picard) your just in time number 1 we have come across a whole in space everything about unknown what do you suggest
pause
echo I have no idea captin
pause
echo just then enterprise is sucked in to the whole
pause
echo %name%....
pause
echo just then Q appears
pause
echo (Q) why captin you have replaced your number 1
pause
echo (Q) well then lets have a bit of fun with him
pause
echo (picard) you will do nothing of the sort
pause
echo (Q) well its only up to you have the entire star fleet command is destroyed you have 1 hour to decide what happens to star fleet you either let me have fun with the new first officer or bye bye starfleet
pause
echo (Q) Q out
pause
echo (picard) %name% listen to me very carefully Q is a ...... odd being just listen to him and will find a way throught this
pause
echo (%name%) yes sir
pause
echo (Q) your hour is up
pause
echo (picard) %name% you know what to do
pause 
echo %name% yes sir
pause
goto Q'sReturn

:Q'sReturn
echo %name% you are starting an adventure do be careful you might cause a domino effect
pause 
echo you are now starting Q's return
pause
echo (Q) you are a particular one %name% you dont think like the other ones the other ones think in a binary format but you....you somehow explore many different options.
pause
goto Q'sReturn2

:Q'sReturn2
