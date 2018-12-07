# Modify-IntelHD-Display-Memory-VRAM

Nowadays, IntelHD is more powerful for Gaming. Some games have been checked hardware minimal requirement before running and it's failed in this phase. Although your IntelHD is strong enough but you cannot run your games because your Display Memory (VRAM) is not enough (default is just 128MB) to pass the test

This script can help you modify VRAM which Windows is detected to pass the test phase before game running

# How To Use:
1. (Default) In this script, i modified to 1024MB VRAM. You just 
  + "Double click" and add registry key 
  + Restart PC
  + Run command (After PC Restarted and login to OS): dxdiag to check your result like this:
  
  ![image](https://user-images.githubusercontent.com/25785573/49632583-ce34c200-fa28-11e8-8e4e-4539edd8e2a1.png)
  
2. Edit the number your want.
  + Open file with notepad
  + Edit the number in "dword:00000400"
  + Attention: why it is 400, not 1024 as i said, because this is HEX Number, not DEC Number. you can use Calculator to convert DEC to HEX and replace number in script. You must make sure the quatity of number after dword: is always 8
  + Save the script and run
  + Restart PC and check again by command dxdiag
