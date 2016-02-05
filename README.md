<h1>GoPro HERO4 Session Scripts</h1>
License: See License File
<p>This archive has a few scripts that will help users of the GoPro HERO4 Session get the most out of their camera. Use at your own risk.</p> 
Holding the Top button > 10seconds will turn off the camera. <br />
Both buttons > 10 seconds will go to factory defaults.<br />

<h2>Hack description</h2>
autoexec.ash was removed in v1.50. We now use the calibration script tunnel. This method works by placing a unix formatted file named 'cal.txt' with the command structure:<br/>
_tapp <test command><br/>
where <test command> is from the ambsh command of 't app'. Supported test commands are seen in "t app.txt" 

<h2>Issues</h2>
cal.txt takes 7 seconds to start running after boot. In one button mode, it may crash your camera. That is why the 'no_shutdown.txt' file exists. You will have to manually start recording after the script has ran if you would like to use the camera in the same session. 

There is no shell commands from this level and 'cal.txt' will still reside after a power cycle. If you are using the 'cal.txt' to set modes, you must manually remove this file yourself.

<h2>Directory Description</h2>
  linux-terminal - Opens up a console to the linux OS via USB. Windows installed driver automatically<br />
  rtos-terminal - Opens up a console to Ambarella Shell. Need a standard CDC USB Serial driver.<br />
  mtp-mode - Resets your GoPro HERO4 Session to MTP mode. (appears as a camera over USB)<br />
  msc-mdoe - Sets your GoPro HERO4 Session as an standard drive. (appears as a drive over USB)<br />
  config - expanded out of config.gz from kernel build<br />
  t* - various test commands available<br />

