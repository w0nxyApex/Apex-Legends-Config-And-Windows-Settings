# Apex Legends Config and Windows Settings

Hi, I'm a seasoned Apex Legends player who has achieved Master rank for many seasons using MNK. I'd like to share my settings and configurations with you, including Windows and NVIDIA settings, to help you achieve an optimal gaming experience without micro stutters and FPS lags. Remember, the effectiveness of these settings can vary based on your system and peripherals.

## Apex Legends Optimization Guide

Welcome to this Apex Legends optimization guide! This repository is designed to enhance your gameplay experience in Apex Legends through detailed configurations and optimizations for video settings, Windows settings, and NVIDIA settings, aimed at reducing micro stutters and FPS lags.

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

- **Particle Levels**: Reduced to ensure minimal distraction and improve performance.
- **Ragdoll Effects**: Disabled to decrease CPU load.
- **Shadow and Lighting Effects**: Minimized to enhance FPS.

[Videoconfig.txt](https://github.com/w0nxyApex/Apex-Legends-Config-And-Windows-Settings/blob/main/videoconfig.txt).

### Autoexec Configuration (`autoexec.cfg`)

The `autoexec.cfg` file pre-loads specific commands to enhance performance and in-game behavior:

- Network optimizations
- Default startup settings
- Graphical adjustments

[autoexec.cfg](https://github.com/w0nxyApex/Apex-Legends-Config-And-Windows-Settings/blob/main/autoexec.cfg).

### Windows Settings

This section will cover various Windows Command Prompt commands to optimize network settings and adjust packet sizes for a smoother online experience. More details will be provided soon.

### NVIDIA 3D Settings

Optimal NVIDIA 3D settings are provided to ensure the best balance between performance and visual fidelity. Keeping your drivers up to date is crucial to avoid any conflicts. Screenshots of these settings will be provided for easier replication.

## Contributing

Contributions are welcome! If you have any tweaks or additional settings that could help improve this guide, please feel free to fork this repository and submit a pull request.

## License

This project
