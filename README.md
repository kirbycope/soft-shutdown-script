# soft-shutdown-script
![Screenshot](/safe-shutdown.png)

## Install the Button
This assumes you use GPIO26 (37) and Ground (39). I wired used a reset switch from an old pc case but just about any momentary switch should do the job.

## Install the Script
1. Open terminal
1. Paste in the following, `wget https://raw.githubusercontent.com/kirbycope/soft-shutdown-script/main/soft_shutdown.py` and then press [Enter]
   - To confirm the file was downloaded, run `ls` to list files in the current directory
1. Paste in the following, `sudo nano /etc/rc.local` and then press [Enter]
1. Scroll down to the end and paste in `sudo python /home/pi/soft_shutdown.py &` above "exit 0
1. Press [Ctrl]+[O] and the press [Enter] to Save
1. Press [Ctrl]+[X] to Exit
1. Type in `sudo reboot' and then press [Enter]
