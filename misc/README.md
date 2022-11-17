Tools have only been tested run from the root directory

`copier` copies a device incremenetly. Within it a function `copy_device` copies the given device, e.g. `copy_device AHU 6` copies AHU-1 into AHU-1, AHU-2, ... AHU-6. Run bin/genkeys after

`pubber_list.txt` (__PUBBER_LIST__)source file for programatically running pubber with given options

`update_list PUBBER_LIST` updates the given __pubber_list__ to addd any missing devices

`runpubber PROJECT_ID PUBBER_LIST` runs sequentially pubber for every device in `PUBBER_LIST` with given options, terminating when one pointset message has been sent

Replay messages with `UDMI/misc/replay_validated/replay`. Create a backup of the validator `out` directory to be replayed first (because validator overwrites out), and launch validator before replayig (because validator removes old messages)