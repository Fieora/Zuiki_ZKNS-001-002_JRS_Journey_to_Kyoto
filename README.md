# Zuiki_ZKNS-011_JRS_Journey_to_Kyoto
This is a quick hack of the original script to work with both Zuiki ZKNS-011 (ZUIKI MasCon for Nintendo Switch RED, probably the blue too).

It is also modified to work with default keyboard bindings since version 1.0.3 of the game.


これは、Zuiki ZKNS-011 

また、ゲームのバージョン 1.0.3 以降のデフォルトのキーボード バインディングで動作するように変更されています。

#### Known bug / 既知のバグ:
If another controller (in my case a PS4 one) is connected at the same time as the ZKNS, the script may duplicate all the inputs and provoke high CPU usage, please be sure to unplug others if you see the logging being flooded.

I suspect it is caused by a drifting joystick, even sightly.

別のコントローラー (私の場合は PS4 コントローラー) が ZKNS と同時に接続されている場合、スクリプトによってすべての入力が複製され、CPU 使用率が高くなる可能性があります。ログがあふれている場合は、必ず他のコントローラーを取り外してください。

見た目にもジョイスティックのドリフトが原因ではないかと思われます。


### Original:

Zuiki "support" for Japanese Rail Sim: Journey to Kyoto via keyboard events.

Required Python packages:  
pyautogui  
pygame  
  
Download the .py file and run via: python.exe .\Zuiki_JRS_Journey_to_Kyoto.py   
Alternatively you can now also download a executable release that was created with py2exe.  
  
At the start you will need to select the line you want to drive, as the train on the Eizan line maps notches differently.  
Once you are in the cabin, sync the controller up by putting it into the EB setting.  
  
The inputs will be buffered, so there is a delay if you move many notches at once.  
This is by design, as the game only accepts keyboard inputs separated by a pause.  

 
 
## Works with steam input enabled 
  
  
Lever and most buttons are working.  
There is no support for the electric brake, as there are not enough notes on the controller.
  
Button mappings:
 

| Controller  | Game |
| :-------------: | :-------------: |
| D-pad left  | D-pad left  |
| D-pad right  | D-pad right  |
| D-pad up   | D-pad up   |
| D-pad down   | D-pad down   |
| A  | Enter (Confirm)  |
| B  | ESC (Cancel)  |
| Y  | Z (Retry)  |
| Home  | Tab(Pause)  |
| L  | L  |
| -  | Music right (pause screen)  |  
| R  | Horn  |  
| ZR  | Horn 2  | 
| ZL | Space (change view)  |  

Horn is hard mapped, as the game still recognizes some of the buttons in game.  
That's why it's also important to use all buttons, with the exception of Home and R, only while the game is paused or in menus.
