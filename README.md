# ESP32 Audio Bridge 🎵🔌

## Project Description

**ESP32 Audio Bridge** is a Windows application that transforms an ESP32 development board into a high-quality 24-bit/48kHz audio interface using Ethernet connectivity instead of traditional USB audio.

download link: https://drive.google.com/drive/folders/1A8JemfHZBqqJSzW8M08InAVVWeKj4rB7?usp=sharing

## 📋 Features

- **Studio-Quality Audio**: 24-bit/48kHz stereo audio streaming
- **Direct Ethernet Connection**: No router required - direct cable connection
- **Low Latency**: ~20ms round-trip using UDP protocol
- **Zero-Installation**: Single EXE file - just run and use
- **System Tray Interface**: Minimal, unobtrusive operation
- **Bi-directional Audio**: Full duplex audio streaming

## 🛠️ Technology Stack

### Windows Application (C#/.NET)
- **Framework**: .NET 6.0
- **Audio Library**: NAudio (WASAPI)
- **UI**: Windows Forms
- **Networking**: System.Net.Sockets

### ESP32 Firmware (C/Arduino)
- **Framework**: ESP-IDF / Arduino Core
- **Audio**: I2S with AC101 codec
- **Networking**: LWIP TCP/IP stack
- **Protocol**: UDP audio streaming

### ESP32 Configuration
1. Flash ESP32 with provided firmware
2. Set static IP: `192.168.1.200`
3. Connect Ethernet cable to PC
4. PC IP: `192.168.1.100`

## 🚀 Usage

1. **Connect**: Ethernet cable between PC and ESP32
2. **Run**: Launch ESP32AudioBridge.exe
3. **Start**: Click "Start Bridge" in application
4. **Control**: Use system tray icon for management
5. **Stream**: Audio automatically flows both directions

## 🎯 Use Cases

- Professional audio streaming
- Multi-room audio systems
- Gaming/VR audio setups
- Studio recording interfaces
- Educational audio projects

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request


## 🙏 Acknowledgments

- NAudio library for Windows audio handling
- Espressif Systems for ESP32 platform
- AC101 audio codec driver contributors


**Note**: Requires ESP32-A1S board with AC101 audio codec and Ethernet connectivity (W5500 module recommended).
