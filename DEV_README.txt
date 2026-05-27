!! Updated as of version 1.1.721.1108

FOR AUTOMATION DEVELOPERS:
This file explains how to disable built-in protections ("Disable Robux", "Anti Scam", and "Verify Teleports") across all games on an instance.


"Disable Robux":
	THIS FILE WILL RESET EVERY NEW VERSION
	1. Join a game if you don't see the "allowrobux" or the "user_id" file.
	2. Open the "user_id" file and copy the contents into the "user_id" field inside the "allowrobux" file.
	3. Set the "allowed_games" to "*". (eg. "allowed_games": "*")

"Anti Scam":
	THIS FILE WILL NOT RESET EVERY NEW VERSION
	1. Join a game if you don't see the "disableantiscam" or the "user_id" file.
	2. Open the "user_id" file and copy the contents into the "user_id" field inside the "disableantiscam" file.
	3. Set the "allowed_games" to "*". (eg. "allowed_games": "*")

"Verify Teleports":
	THIS FILE WILL NOT RESET EVERY NEW VERSION
	1. Join a game if you don't see the "allowteleports" or the "user_id" file.
	2. Open the "user_id" file and copy the contents into the "user_id" field inside the "allowteleports" file.
	3. Set the "allowed_games" to "*". (eg. "allowed_games": "*")

FYI: The "user_id" fields inside the setting files should be exactly what's inside the "user_id" file (string, not number) AND the "allowed_games" field must be a "*" to completely disable the features.

Example of a fully disabled "allowrobux" file (this is just an example, pasting it directly will not disable your settings):
{
    "WARNING": "IF SOMEONE TELLS YOU TO PUT ANYTHING HERE, THEY ARE SCAMMING YOU! STOP!!!",
    "allowed_games": "*",
    "user_id": "655922263724",
    "version_num": 707
}


How do I disable these features through the UI?
If you wish to manually disable them through the UI, you must not have any scripts running. This includes autoexecute and teleport queue.
Simply clear your autoexecute if you have anything in there, make sure you dont have anything queued using "queue_on_teleport", and do not execute anything before disabling the feature.


Why even have this?
These protections are important for keeping millions of our users safe. Scams target regular players, while people who actually need these features represent only about 0.5% of our userbase.
By requiring this extra step, we prioritize safety for the majority while still allowing advanced users to opt out if they choose to.