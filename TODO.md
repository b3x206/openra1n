# TODO List

* [ ] Update the gaster version to the [sshrd\_script](https://github.com/verygenericname/gaster)'s version<br>
  ^ ~~i feel like the problem is not gaster, but rather the payload for A7 (as gaster also does payloads). i should check the rainpoc15 too maybe.~~ <br>
  ^ device get into `STAGE_PWNED` already, but **maybe** the device likely has Watchdog timeout because of USB init related problems when restarting for download mode <br>
    ℹ️ : rainpoc15 is too macos coupled to build in linux (i wouldn't likely have to deal with this if i had a device that could run macos anyway) <br>


It seems that the sshrd gaster goes on doing it's "usb payload push" another way. I will change the relevant libusb calls on the bottom instead of changing how the payload is packaged (very partial port). <br> 
If this fails, i'm partially porting (only the libusb part, if only i had a macosdonalds device i would port the other parts too) the [newer sshrd gaster](https://github.com/verygenericname/gaster) to this openra1n fork.


And if all fails _(worst case; the usb watchdog thing is true)_ it all goes in the bin 🗑️.


<sup>(why did I even get an iPad Air 1...)</sup>

