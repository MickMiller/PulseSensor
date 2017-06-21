In this dir are programs developed before PulseSensor.ino
    
Setup:
  Purple lead to analog A0
  Red lead to 3-5V (available on Arduino)
  Black to Gnd (available on Arduino)
  Arduino board (USB mini) to laptop (USB)
  Invoke Arduino App
    Access program (Tech\Automation\AutomationProject\Phase2Programs\Programs\PulseSensor\PulseSensor.ino)
    Upload
    Invoke Serial Monitor (Tools > Serial Monitor)
	Put twofingers on sensor
  Expected Results is list, eg "Beats Per Minute: 54"

  
The most valueable lesson learned is "Know thy data".  Once raw Signal
displayed development was quick.

Note this is a prototype so some adjustment of sensor on finger may be
needed.

Now there is one filter - keep sensor counts above 550.  Other filters
could be added:
- Measure width of pulse when sensor reading is over 550.  Only keep pulse of
  appropriate width (eg 1/8 sec).
- Rise count of more than 50.
- Rise time over 1/8 sec