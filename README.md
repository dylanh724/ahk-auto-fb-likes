; ahk-auto-fb-likes (fblike.ahk)

; Summary: CTR+SHIFT+L will invite 50 people on your FB page to "Like" your page, automatically.

; Created by dylanh724@gmail.com on 1/25/2016

; Freely distributed via MIT license

; ####################################################################

; 1) Double click fblike.ahk

; 1b) Alternately, start w/Windows

; 2) Go to a page you want to invite people to "Like" on FB

; 3) Scroll down many times to load up a bunch of people to "invite

; 4) From as far down as possible, "Invite" 1 person

; 5) Finally, CTRL+SHIFT+L to invite 50 people on the list

; IMPORTANT: ESC to cancel!! If you click outside, do press ESC ASAP.

; NOTE 1: To change how many is invited, change the "Loop 50" below

; NOTE 2: Why does this go backwards? Because it's consistent enough
;         to make a hotkey. Going forwards seems unpredictable.

; IF UPGRADED: I use this myself, so please let me know so I can use
;              your better version ;)

; ####################################################################

	^+L::

		Loop 50 {
		
		   Send, +{tab 3}
		   
		   Send, {Enter}
		   
		   sleep, 1000
		   
		}   
	
		Return

	Escape::

		ExitApp
		
		Return
