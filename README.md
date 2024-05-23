# Apex-Legends-Config-And-Windows-Settings
Hi, about me, I was Master in Apex for many seasons on MNK. I'd like to share my settings and config with you here, as well as my Windows settings and NVIDIA settings for an optimal gaming experience without micro stutters and FPS lags. Of course, it always depends on your system and peripherals as well.

Apex Legends Optimization Guide

Welcome to my Apex Legends optimization guide! This repository contains detailed information and configurations to enhance your gameplay experience in Apex Legends. You will find optimizations for video settings, Windows, and NVIDIA configurations aimed at reducing micro stutters and FPS lags.
Video Configuration (videoconfig.txt)

This section explains the purpose and effects of various settings in the videoconfig.txt file. Adjusting these settings can significantly improve game performance and visual quality.

Key settings include:

    Particle Levels: Reduced to ensure minimal distraction and improve performance.
    Ragdoll Effects: Disabled to decrease CPU load.
    Shadow and Lighting Effects: Minimized to enhance FPS.

You can view the detailed configuration here.
Autoexec Configuration (autoexec.cfg)

The autoexec.cfg file allows you to pre-load specific commands that enhance performance and behavior in-game. It includes:

    Network optimizations
    Default startup settings
    Graphical adjustments

Details of these commands can be found in the autoexec.cfg file.
Windows Settings

This section will cover various Windows Command Prompt commands to optimize network settings and adjust packet sizes for a smoother online experience. Details will be added soon.
NVIDIA 3D Settings

Optimal NVIDIA 3D settings are provided to ensure the best balance between performance and visual fidelity. It is crucial to keep your drivers up to date to avoid any conflicts. Screenshots of these settings will be provided for easier replication.
Steam Game Launch Options

Customize your game launch options in Steam to fine-tune performance and user experience. Here are some recommended commands:

Command	Description
+exec	Executes a cfg file on startup
-dev	Skips EA intro on startup, can cause HUD flicker issues on NVIDIA cards
-fullscreen	Forces the game to launch in fullscreen mode
-high	Gives high priority to the game in system processes
-preload	Preloads game assets
-forcenovsync	Disables vertical sync
-m_rawinput 1	Ensures raw input is used for mouse movements

Full command line example: -high -preload -forcenovsync -dev -fullscreen +exec autoexec.cfg -m_rawinput 1
Contributing

Contributions are welcome! If you have any tweaks or additional settings that could help improve the guide, please feel free to fork this repository and submit a pull request.
License

This project is released under the MIT License. See the LICENSE file for more details.
Contact

For further assistance or to provide feedback, feel free to contact me [insert your contact information or link to your GitHub profile].
