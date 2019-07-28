# Wilma Head of Train Device (HOTD)

![Build-Status](https://img.shields.io/badge/build-passed-brightgreen.svg)
![Manifest-Version](https://img.shields.io/github/last-commit/titus-studios-media/Wilma-Head-of-Train-Device.svg)
![Repo-Size](https://img.shields.io/github/repo-size/titus-studios-media/Wilma-Head-of-Train-Device.svg)

A "dumb" ETD can be as simple as a red flag attached to the coupler on the last car of the train, whereas "smart" devices monitor functions such as brake line pressure and accidental separation of the train using a motion sensor, functions that were previously monitored by a crew in the caboose. The ETD transmits data via a telemetry link to the Head-of-Train Device (HTD) in the locomotive, known colloquially among railroaders as a "Wilma", a play on the first name of the wife of cartoon character Fred Flintstone. In Canada, this device is known as a sense and braking unit (SBU).

A typical HTD contains several lights indicating telemetry status and rear end movement, along with a digital readout of the brake line pressure from the ETD. It also contains a toggle switch used to initiate an emergency brake application from the rear end. In modern locomotives, the HTD is built into the locomotive's computer system, and the information is displayed on the engineer's computer screen.

Railroads have strict government-approved air brake testing procedures for various circumstances when assembling trains or switching out cars en route. After a cut is made between cars in a train and the train is rejoined, in addition to other tests, the crew must verify that the brakes apply and release on the rear car (to ensure that all of the brake hoses are connected and the angle cocks, or valves, are opened). In most cases, the engineer is able to use information from the ETD to verify that the air pressure reduces and increases at the rear of the train accordingly, indicating proper brake pipe continuity. This device is said to constitute a fail-safe condition.

# New Features

This is the "Version 2" of my previous HOTD E2, some of the improvements are;

 * Simulated "Slowness" of the Brake Pipe (delayed pressure gain and release from the last car, more realism)
 * New Data Transfer System
 * Quicker Setup Time and Installation
 * Newer Radio Break Function
 * Fixed Accelerometer
 * Wireless / Radio Function
 * Lower OPS and CPU time (Less laggy and less hard on the server)
 * Rear Car Emergency Function (Yes it actually works)
 * Fixed Many Bugs
 * [New and Updated EOTD Expression 2](https://github.com/titus-studios-media/TrainLink-II-ATX-End-Of-Train-Device) - https://github.com/titus-studios-media/TrainLink-II-ATX-End-Of-Train-Device


# Installation

1. Click the "Clone or Download" button on the righthand side of the screen and select "Download Zip."
2. Open the Zip file using a program like WinZip or WinRar, if it didn't open automatically.
3. Navigate __INTO__ the "wilma-head-of-train-device-master" Folder. You should see two items: a file named "titus's_wilma_head_of_train_device_(HOTD).txt", and readme.md.
4. Extract the two folders directly into: `<Your active steam directory>\SteamApps\common\Garry's Mod\garrysmod\data\expression2\`.
The file path should then look like `expression2\titus's_wilma_head_of_train_device_(HOTD).txt`.

You will also need Magnums Train Models, Titus's Locomotive Sound Expansion Pack's Sound packs and Proppertextures for it to work correctly. There are seven:

Titus's Locomotive Sound Expansion Pack(s):

 * https://steamcommunity.com/sharedfiles/filedetails/?id=1572612341
 * https://steamcommunity.com/sharedfiles/filedetails/?id=1572613783
 * https://steamcommunity.com/sharedfiles/filedetails/?id=1572616038
 * https://steamcommunity.com/sharedfiles/filedetails/?id=1572620031
 * https://steamcommunity.com/sharedfiles/filedetails/?id=1797390076
 
Magnum's Train Model Pack
 * https://steamcommunity.com/sharedfiles/filedetails/?id=260954002
 
Grovesteetgman's The Big Propper Train Shared Texture Pack (Proppertextures)
 * https://steamcommunity.com/sharedfiles/filedetails/?id=1227050421

If you're currently in-game in Garry's Mod, open the E2 Editor, and click the "Update" button under the list of E2s on the left hand side of the window.


# Wiring

To Wire:
1. Begin by spawning the E2 on the ground, and placing it somewhere in the Locomotive.
2. Wire `RLCPT[ENTITY]` to the RLC Gamma (PT2) Chip
3. Wire `On` to the MU or Battery Switch
4. (Optional), Wire `Emergency` to a button or key to enable you to apply the Emergency from the rear car.

**NOTE:** This E2 can be Parented!


# Usage

To use the E2, power it up, then the displays should begin flashing; This means the EOTD is not linked to the HOTD, also known as "Radio Break".

To link the EOTD:
1. First spawn the compatible EOTD E2 *[(Find it here)](https://github.com/titus-studios-media/TrainLink-II-ATX-End-Of-Train-Device)*
2. Wire the `Railcar[ENTITY]` to the Railcar (or Locomotive) you wish to attach the EOTD to, this allows the EOTD's Emergency Function to... Function. **However it is not required.**
3. Get out your Crowbar, and press "E" while looking at the EOTD, this is the Power and mode selector. Press once to start the EOTD with no flashing light, Press it again to make the light flash, and one more time to power the EOTD down.
4. To actually link it, you can either; Wire it (Manually), or use the built in "Wireless / Radio" Mode.

**NOTE:** The old EOTD Expression 2 is NOT compatible with this!

To use the "Wireless / Radio" Mode;
1. Look at the EOTD
2. Type in chat `//link eotd` or `//link eot`
3. A notification should pop up on your screen saying that it linked correctly.

To Un-Link Type; `//unlink eotd` or `//unlink eot`

**NOTE:** The linking function will ONLY work if you are looking at the EOTD (centre of your screen), this also goes for un-linking.

**NOTE:** The linking function does not work if the EOTD is parented. Link it first before you parent it.


# Verifying Connection

To Verify that the link worked, head to the HOTD and see if the displays are still flashing, if they are not, and it is displaying the PSI on the last car (Depends on if the Trainline brake is applied or not), if not, then go back to the EOTD, type `//unlink eotd` or `//unlink eot`, and try re-linking again.


#### You're Done!


# Thank You!
Thank you for installing Titus's Wilma Head of Train Device Expression 2.
Find my other work around the internet:
 * [Website](https://titusstudiosmediagroup.github.io/) | https://titusstudiosmediagroup.github.io/
 * [Twitter](https://twitter.com/TitusStudiosMG) | https://twitter.com/TitusStudiosMG
 * [Twitch](https://www.twitch.tv/titusstudios) | https://www.twitch.tv/titusstudios
 

Copyright © 2019 Titus Studios Media. All rights reserved. Contact Titus Studios Media, for more information or licencing.


