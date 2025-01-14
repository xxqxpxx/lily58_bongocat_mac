Lily58 macos + BongoCat + WPM + Layer Indicator + custom layout
A customized Lily58 keyboard configuration featuring BongoCat animation, WPM counter, and layer indication.


Prerequisites
This configuration is designed for:

Lily58 Pro keyboard
Arduino Pro Micro (or compatible clone) microcontrollers
No RGB or underglow modifications
Left-side master configuration

Features
OLED Displays

Left Display: Shows current WPM and active layer
Right Display: Features BongoCat animation that responds to typing speed

Below 30 WPM: Idle animation
At 30 WPM: Raised arms
40+ WPM: Animated table tapping



Note: The WPM counter is intended for fun rather than accurate typing speed measurement.
Keyboard Layout
Base Layer (QWERTY)


,-----------------------------------------.                    ,-----------------------------------------.
| ESC  |   1  |   2  |   3  |   4  |   5  |                    |   6  |   7  |   8  |   9  |   0  |  =   |
|------+------+------+------+------+------|                    |------+------+------+------+------+------|
| Tab  |   Q  |   W  |   E  |   R  |   T  |                    |   Y  |   U  |   I  |   O  |   P  |  -   |
|------+------+------+------+------+------|                    |------+------+------+------+------+------|
|fn/Cmd|   A  |   S  |   D  |   F  |   G  |-------.    ,-------|   H  |   J  |   K  |   L  |   ;  |  '   |
|------+------+------+------+------+------|  [/L3  |    |  ]/L3 |------+------+------+------+------+------|
|LShift|   Z  |   X  |   C  |   V  |   B  |-------|    |-------|   N  |   M  |   ,  |   .  |   /  |RShift|
`-----------------------------------------/       /     \      \-----------------------------------------'
                   | Ctl |  Opt  | Cmd  | /Sp/L2  /       \Enter \  |Bp/Cmd|Dl/Opt| Ctl  |
                   |     |       |      |/       /         \      \ |      |      |      |
                   `----------------------------'           '------''--------------------'




Navigation Layer (Layer 2)

,-----------------------------------------.                    ,-----------------------------------------.
| ESC  |      |ShCmd2|ShCmd3|ShCmd4| Home |                    |      | Prev | Play | Next | Mute |VolUp |
|------+------+------+------+------+------|                    |------+------+------+------+------+------|
| Tab  |      |  ←   |   ↑  |   →  |PgUp |                    |      |  ←   |   ↑  |   →  |      |VolDn |
|------+------+------+------+------+------|                    |------+------+------+------+------+------|
|fn/Cmd|      |      |   ↓  |      |PgDn |-------.    ,-------|   ~  |   |  |   :  |   .  |   \  |  '   |
|------+------+------+------+------+------|  [/L3  |    |  ]/L3|------+------+------+------+------+------|
|LShift|      |      |      |      | End |-------|    |-------|      |      |      |      |      |RShift|
`-----------------------------------------/       /     \      \-----------------------------------------'
                   | Ctl |  Opt  | Cmd  | /Space /       \Enter \  |BckSp |  Del | Ctl  |
                   |     |       |      |/      /         \      \ |      |      |      |
                   `---------------------------'           '------''--------------------'



Function Layer (Layer 3)
,-----------------------------------------.                    ,-----------------------------------------.
| ESC  |  F1  |  F2  |  F3  |  F4  |  F5  |                    |  F6  |  F7  |  F8  |  F9  | F10  | F11  |
|------+------+------+------+------+------|                    |------+------+------+------+------+------|
| Tab  |   *  |   1  |   2  |   3  |  +   |                    |MWhlUp|MLeft |  MUp |MRight|      | F12  |
|------+------+------+------+------+------|                    |------+------+------+------+------+------|
|fn/Cmd|   /  |   4  |   5  |   6  |  -   |-------.    ,-------|MWhlDn|MLeft |MDown |MRight|PrtSc |  '   |
|------+------+------+------+------+------|  [/L3  |    |  ]/L3 |------+------+------+------+------+------|
|LShift|   ^  |   7  |   8  |   9  |   .  |-------|    |-------|Insert|Pause |ScrLk |NumLk |PrtSc |RShift|
`-----------------------------------------/       /     \      \-----------------------------------------'
                   | Ctl |  Opt  | Cmd  | /  0   /       \Enter \  |BckSp |  Del | Ctl  |
                   |     |       |      |/      /         \      \ |      |      |      |
                   `---------------------------'           '------''--------------------'



Known Issues and Future Improvements

OLED Sleep Timing: The left and right OLED displays currently have different sleep timeouts. Future updates will synchronize their sleep/wake behavior.

Installation

Clone this repository
Replace your existing keymap.c with the one provided (or reference the original layout from previous commits)
Compile and flash to your Lily58 Pro

Contributing
Feel free to submit issues and enhancement requests!

this layout is following the work of u/jwoolson24 and some changes to fit my style from 
https://www.reddit.com/r/ErgoMechKeyboards/comments/1aqrbth/macos_qwerty_layout_for_lily58_allium58_with_a/
