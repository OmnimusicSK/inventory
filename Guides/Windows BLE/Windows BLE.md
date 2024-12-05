# Using BLE devices on Windows (10+)

## Guide

Unfortunately, unlike MAC and iOS, there is no native support (as of 5/12/24) for BLE (Bluetooth Low Energy) MIDI devices in Windows. This may change but is unlikely to happen quickly.

To successfully use a BLE MIDI device in windows, 2 pieces of software are required:

- A BLE MIDI connection manager (MIDI Berry is recommended)

- A MIDI Loopback port manager (loopMIDI is recommended)

The BLE MIDI connection manager will actually handle connecting your bluetooth device, but the data it sends needs somewhere to go! The loopback port manager handles creating virtual MIDI ports for sending data to other programs, like Ableton.


You can download loopMIDI [here](https://www.tobias-erichsen.de/software/loopmidi.html).

You can download MIDIBerry [here](https://apps.microsoft.com/detail/9n39720h2m05?rtc=1&hl=en-gb&gl=GB). Alternatively, you can search for it on the microsoft store (type "store" in the start menu).

Once you have installed loopMIDI, open it. Type any name in the text box in the lower right (We suggest "BLE MIDI") and click the "+" button in the lower left corner to create a virtual port. You can create as many as you like, and name them as you want.

Ensure your bluetooth is turned on (Type "bluetooth" in the start menu - you should have "Bluetooth and other devices settings"), then ensure bluetooth is switched "on".

Next, we have to connect to our BLE MIDI device. In "Bluetooth and other devices settings", select "Add bluetooth or other device", then "Bluetooth: Mice, keyboard, pens, etc...". Select your device when it appears and it should eventually show as "connected" in the bluetooth devices list.

Now, opening MIDIBerry, you should see a list of input and output devices. Select your BLE device as the input, and your loopMIDI port as the output.

Now MIDI data is being sent to the loopMIDI port, you can use it as a MIDI input in your DAW or other software.

Be careful about sending MIDI "out" to the loopMIDI port! This could result in an infinite loop where data is being sent out of your output and back in again at the input.


## Troubleshooting

Having other issues? [ask a question](<mailto:ChrisBall@omnimusic.org.uk>)

