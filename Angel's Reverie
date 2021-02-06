#maxThreadsPerHotkey, 3
setKeyDelay, 50
setMouseDelay, 50
autogrinder:=0
autoworder:=0
autoword:=0
autogrinderrepeats:=0
enabled:=false
MsgBox, Angel's Reverie v.1.1.0`nScript is ready to activate, Alt + F1 to toggle script`nShift+F1 to toggle Auto Excube-to-Grinder.`nShift+F2 to toggle Autoword.
Suspend, On

!f1::
Suspend, Permit
{
	if (enabled=true)
	{
		MsgBox, Script disabled.
		IfMsgBox, OK
		{
		SplashTextOff
		Suspend, On
		}
	}
	else if (enabled=false)
	{
		MsgBox, Script enabled.
		IfMsgBox, OK
		{
		SplashTextOff
		Suspend, Off
		}
	}
	enabled:=!enabled
}
return

+1::
{
	Send {Numpad1}
	SplashTextOn, , , Switched to Weapon 1.
	Sleep, 250
	SplashTextOff
}
return

$+f1::
#MaxThreadsPerHotkey 2
{
	autogrinder:=!autogrinder
	
	if (autogrinder=1) 
	{
		MsgBox, Auto Excube to Grinder enabled. 
		SplashTextOn, , , Executing...
	}
	else if (autogrinder=0) 
	{
		MsgBox, Auto Excube to Grinder disabled. 
		SplashTextOn, , , Stopping. Please wait for last loop...
	}
	
	
while (autogrinder=1)
    {
		Send {Enter} ; open shop     change to suit your ping and pc
		Sleep, 1800
		Send {Left} ; maxbuy grinders
		Sleep, 200
		Send {Enter} ; purchase
		Sleep, 300
		Send {Enter} ; purchase     change to suit your ping and pc
		Sleep, 450
		Send {Escape} ;
		Sleep, 300
		Send {Escape} ;
		Sleep, 300
		Send {Up} ; 
        Sleep, 200
        Send {Up} ; select storage
		Sleep, 200
		Send {Enter} ; open storage
		Sleep, 300
		Send {Enter} ; deposit
		Sleep, 300
		Send {Enter} ;
		Sleep, 300
		Send {Enter} ;
		Sleep, 300
		Send {Enter} ; deposit to storage
		Sleep, 300
		Send {Down} ; character storage     change to select which storage you use
		Sleep, 200
		Send {Enter} ; deposit
		Sleep, 200
		Send {Right} ; max
		Sleep, 200
		Send {Enter} ; deposit
		Sleep, 300
		Send {Enter} ; deposit
		Sleep, 350
		Send {Escape} ; 
		Sleep, 350
		Send {Escape} ; 
		Sleep, 350
		Send {Escape} ; 
		Sleep, 350
		Send {Down} ; shop
		Sleep, 200
		Send {Down} ; shop
		Sleep, 200
		if (autogrinder=0)
		{ 
		SplashTextOn, , , Stopping...
		Sleep, 1000
		SplashTextOff
		}
		else
		{
		SplashTextOn, , , Repeating...
		}
	}
	autogrinder:=false
}
return

$+f2::
#MaxThreadsPerHotkey 2
{
	autoworder:=!autoworder
	if (autoworder=1) 
	{
		MsgBox, Autoword enabled.
		SplashTextOn, , , Executing.
	}
	else if (autoworder=0) 
	{
		MsgBox, Autoword disabled.
		SplashTextOn, , , Stopping.
		Sleep, 500
		SplashTextOff
	}
	
	
while (autoworder=1)
    {
		Random, autoword, 1, 18
		Send {Enter}
		if (autoword=1)
		{
			Send guh
		}
		if (autoword=2)
		{
			Send uwu
		}
		if (autoword=3)
		{
			Send kyan
		}
		if (autoword=4)
		{
			Send x3333
		}
		if (autoword=5)
		{
			Send ib.
		}
		if (autoword=6)
		{
			Send dropkick
		}
		if (autoword=7)
		{
			Send omori
		}
		if (autoword=8)
		{
			Send vtuber
		}
		if (autoword=9)
		{
			Send pso2
		}
		if (autoword=10)
		{
			Send ichi ni san shi go fun
		}
		if (autoword=11)
		{
			Send toki doki honto ni netai
		}
		if (autoword=12)
		{
			Send close your eyes you'll be here soon
		}
		if (autoword=13)
		{
			Send demo kono waado dekinai
		}
		if (autoword=14)
		{
			Send oyasumi
		}
		if (autoword=15)
		{
			Send close your eyes and you'll leave this dream
		}
		if (autoword=16)
		{
			Send ooooyasumi
		}
		if (autoword=17)
		{
			Send okakugo
		}
		if (autoword=18)
		{
			Send dream
		}
		Send {Enter}
		Sleep, 800
	}
	autoworder:=false
}
return
