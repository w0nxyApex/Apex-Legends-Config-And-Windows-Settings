# Apex Legends Config and Windows Settings

Hi, I'm a seasoned Apex Legends player who has achieved Master rank for many seasons using MNK. I'd like to share my settings and configurations with you, including Windows and NVIDIA settings, to help you achieve an optimal gaming experience without micro stutters and FPS lags. Remember, the effectiveness of these settings can vary based on your system and peripherals.


#### By the way, it doesn't make any difference how good your settings and fps are - almost every console player with 0.6 AA will outgun you. Aloo have fun :)


I also got some of my settings from these people. //github.com/V3nilla, //github.com/kretz1xD, //github.com/deaFPS So stop by if you're interested.


## Apex Legends Optimization Guide

This repository is designed to enhance your gameplay experience in Apex Legends through detailed configurations and optimizations for video settings, Windows settings, and NVIDIA settings, aimed at reducing micro stutters and FPS lags.



### Steam Game Launch Options

To optimize your gameplay, add the following commands to your launch options in Steam:

| Command          | Description |
|------------------|-------------|
| `+exec`          | Executes a cfg file on startup |
| `-dev`           | Skips EA intro on startup, can cause HUD flicker issues on NVIDIA cards |
| `-fullscreen`    | Forces the game to launch in fullscreen mode |
| `-high`          | Gives high priority to the game in system processes |
| `-preload`       | Preloads game assets |
| `-forcenovsync`  | Disables vertical sync |
| `-m_rawinput 1`  | Ensures raw input is used for mouse movements |

Example of full command line: `-high -preload -forcenovsync -dev -fullscreen +exec autoexec.cfg -m_rawinput 1`


### Video Configuration (`videoconfig.txt`)
This section explains the purpose and effects of various settings in the `videoconfig.txt` file to improve game performance and visual quality:


Adjust the following in your `videoconfig.txt` for optimal frame timing:
- **Original Frame Time**:
  - Minimum: `"15000"`
  - Maximum: `"15000"`
  - Optimal for 190 FPS: "setting.dvs_gpuframetime_min"	`"5150"`
                         "setting.dvs_gpuframetime_min"	`"5150"`
  - Optimal for 240 FPS: "setting.dvs_gpuframetime_min" `"4166"`
                         "setting.dvs_gpuframetime_min"	`"4166"`     
  - Optimal for 299 FPS: "setting.dvs_gpuframetime_min" `"3340"`
                         "setting.dvs_gpuframetime_min"	`"3340"`

- **Particle Levels**: Reduced to ensure minimal distraction and improve performance.
- **Ragdoll Effects**: Disabled to decrease CPU load.
- **Shadow and Lighting Effects**: Minimized to enhance FPS.

[Videoconfig.txt](https://github.com/w0nxyApex/Apex-Legends-Config-And-Windows-Settings/blob/main/videoconfig.txt).
You can simply copy my Videoconfig.txt and use it and replace yours with it. But check which fps you are playing at to set the correct frame times.
and set the file to read only otherwise the game will change settings again.


### Autoexec Configuration (`autoexec.cfg`)

The `autoexec.cfg` file pre-loads specific commands to enhance performance and in-game behavior:

- Network optimizations
- Default startup settings
- Graphical adjustments

[autoexec.cfg](https://github.com/w0nxyApex/Apex-Legends-Config-And-Windows-Settings/blob/main/autoexec.cfg).

## Windows Settings

### Ultimate Performance Mode in Windows

#### Overview
The Ultimate Performance Mode in Windows optimizes power settings to enhance system performance. This mode is particularly beneficial for workstations and users requiring maximum performance from their systems.

#### Activation Command

To activate Ultimate Performance Mode, which is not visible by default in Windows, use the following command in your command prompt:

```bash
powercfg -duplicatescheme e9a42b02-d5df-448d-aa00-03f14749eb61
```
This command duplicates the hidden Ultimate Performance power scheme, enabling it for selection.
Enabling Ultimate Performance Mode

After running the command, follow these steps to activate the Ultimate Performance Mode:

    Open Control Panel.
    Navigate to Hardware and Sound > Power Options.
    Under Choose or customize a power plan, select Ultimate Performance.

Important Notes

    The Ultimate Performance mode is recommended for users who require maximum performance from their systems and is particularly useful on workstations.
    Power Consumption: Be aware that enabling Ultimate Performance Mode may increase your system's power consumption significantly.
    Recommended Use: This mode is recommended for users who need to maximize their system performance and is not typically necessary for general computing tasks.

This format provides clear instructions and essential details, making it easy for users to understand and implement Ultimate Performance Mode. Adjust the steps as necessary to align with specific user environments or system configurations.

### Improve Internet performance with the right MTU size

#### Calculating the Optimal MTU Size

To determine the optimal MTU size without packet loss, use the `ping` command. Start with a high MTU size and adjust as necessary:

```bash
ping 8.8.8.8 -f -l 1492
```

This command pings google.com with a specific packet size (1492 bytes) while setting the "Don't Fragment" flag.


#### Checking Your Current MTU Size

To view the current MTU size for all network interfaces on your system, use the following command:

```bash

netsh interface ipv4 show subinterfaces
```

#### Setting the MTU Size

To set the MTU size for a specific network interface (e.g., Ethernet), use the following command:

```bash
netsh int ipv4 set subinterface "Ethernet" mtu=1500 store=persistent
```

This command sets the MTU size to 1500 for the Ethernet interface and makes the change persistent across reboots. And make sure you have chosen your largest MTU size that will be displayed without being fragmented. 1500 is maximum.
here is a video from someone (https://www.youtube.com/watch?v=RK2PHpKI9M4)

Notes

    Adjust the MTU values based on your specific network conditions and requirements.


Make sure to replace "Ethernet" with the actual name of your network interface if it differs, and adjust the MTU values as necessary based on the results of your MTU size calculation.

#### Windows instalation
I would highly recommend that you watch this video before you reinstall your PC next time. Then you have a better Windows installation.([Video](https://www.youtube.com/watch?v=XQAIYCT4f8Q&list=WL&index=6))

### NVIDIA 3D Settings

Optimal NVIDIA 3D settings are provided to ensure the best balance between performance and visual fidelity. Keeping your drivers up to date is crucial to avoid any conflicts. Screenshots of these settings will be provided for easier replication.

## Contributing

Contributions are welcome! If you have any tweaks or additional settings that could help improve this guide, please feel free to fork this repository and submit a pull request.

## License

This project
