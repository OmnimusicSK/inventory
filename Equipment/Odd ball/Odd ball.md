# Odd ball

<img src="https://oddballism.com/cdn/shop/files/ball_test.png" alt="picture of the odd ball" width="300"/>

Manufacturer Website Link: [Odd Ball](<https://oddballism.com/>)

Serial No(s): 

## Quick Start Guide

Download the Odd Ball app from the [app store (iPhone)](<https://apps.apple.com/us/app/odd-ball/id1453989732>) or [google play store (Android)](<https://play.google.com/store/apps/details?id=com.oddballism.app&hl=en_GB&gl=US>).

Run the app and follow the on-screen instructions. There may be a firmware update.

There are many different modes and ways the odd ball can be used. Unfortunately, the app is much less useful than it used to be, and appears to only focus on limited interaction with preset songs. There are no "sample" or loop modes anymore.

You can also connect the ball directly to music software as a BLE MIDI device (easiest on mobile devices and Mac). The ball sends "note ons" when tapped and and a bunch of other data detailed [here](<https://docs.google.com/document/d/14L2wokwEkl3OIqeRpiXxA0IOLzT7xJSZx7kKNLflzVw/edit?tab=t.0>), but may not be accurate. WARNING: some of the data sent is on CC7, which in the midi specification is volume control on many MIDI devices. This may result in unexplained silence. It should be possible to filter these messages in most DAWs.

As of 19/12/24 the CC parameters are:

| Channel | CC Number | Gesture        |
| ------- | --------- | -------------- |
|    1    | 0         | Shake          |
|    2    | 1 		  | Twist          |
|    1    | 2         | Freefall       |
|    1    | 3         | X Orientation  |
|    1    | 4         | Y Orientation  |
|    1    | 5         | Z Orientation  |
|    1    | 6         | Movement       |


There are some odd ball tutorials, but as this a developing product, the instructions may be out of date:
[Odd ball Tutorials](<https://www.youtube.com/watch?v=T8LEMCSyrb8&list=PLl8Qj7n4CyirhV5Oy4bBT8HhRq_gw9aU3>)

## Troubleshooting

If the Odd Ball does not respond when trying to connect, make sure it is charged. There is no on/off switch - the device simply switches out of standby when it detects movement. As a result it may lose charge quickly.

On Windows, third party pieces of software need to be installed - See our full guide to using BLE devices on windows (it's surprisingly difficult) [here](https://omnimusicsk.github.io/inventory/Guides/Windows%20BLE/Windows%20BLE.html)

Having other issues? [ask a question](<mailto:ChrisBall@omnimusic.org.uk>)
