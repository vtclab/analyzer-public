# Media Analyzer
The purpose of this repository is to provide a communication channel between the authors and the users of VTCLab Media Analyzer app (https://media-analyzer.pro)

In particular:
* To provide basic information about the application features and updates
* To gather feedback from the users (questions, problems, etc.)
* To discuss the ideas and upcoming changes

Currently, analyzer is in the "Public Beta" stage, so don't be surprised if you spot something weird. If you do though, please, send us a message at analyzer@vtclab.com or open an issue here in GitHub.

### Contents
 
[Screenshots](#screenshots)     
[Basic features](#basic-features)    
[Important notes](#important-notes)   
[Feedback](#feedback)     
[Donate](#donate)   
[Version history](#version-history)

## Screenshots

<a href="https://user-images.githubusercontent.com/87360808/212826742-b8f7306e-fe32-4e9d-8566-ec3e51f5602d.png"><img width="100" alt="Screenshot 1" src="https://user-images.githubusercontent.com/87360808/212826742-b8f7306e-fe32-4e9d-8566-ec3e51f5602d.png"></a>
<a href="https://user-images.githubusercontent.com/87360808/212827399-aeb04aed-f8c8-4894-997b-a33fdb653085.png"><img width="100" alt="Screenshot 2" src="https://user-images.githubusercontent.com/87360808/212827399-aeb04aed-f8c8-4894-997b-a33fdb653085.png"></a>

## Basic features

|Containers supported|Comments|
| --- | --- |
| [MPEG-TS](/DETAILS.md#mpeg-ts) | Parsing of TS packets, PAT/PMT & several other tables, PES packets and elementary streams inside them (if corresponding encoding is supported, see below), some descriptors, many DVB descriptors & PSI tables |
| [ISOFF / MP4 / MOV / QuickTime](DETAILS.md#mp4mov) | Parsing of atom/box structure, display the contents of many known atoms/boxes. Show access units of AAC/AVC/HEVC/VVC streams |
| Elementary | Most of the audio/video streams listed below are also supported as elementary streams |
| | |
| **Audio streams supported** |  |
| MPEG-1 Audio (ISO/IEC 11172-3)| Frame headers |
| MPEG-2 Audio (ISO/IEC 13818-3)| Frame headers |
| AAC Audio (ISO/IEC 13818-7, 14496-3)| Frame headers |
| Dolby AC-3, E-AC-3 (ATSC A/52)| Frame headers |
| SMPTE-302M Audio | Frame headers |
| | |
| **Video streams supported** | |
| MPEG-1 Video (ISO/IEC 11172-2) | All headers except slice data and below |
| MPEG-2 Video (ISO/IEC 13818-2) | All headers except slice data and below |
| H.264/AVC Video | Location and types of NAL units, detailed description of basic NAL units|
| H.265/HEVC Video | Location and types of NAL units, detailed description of basic NAL units |
| H.266/VVC Video | Location and types of NAL units, detailed description of VPS/SPS/PPS headers |
| | |
| **Common abilities** | |
| Packet filtering | Each stream has three-state mode selector: <ul><li>**Not selected** (???) - headers from this stream won't be displayed in the list</li><li>**Selected, this stream only** (???) - headers will be displayed, without contained streams</li><li>**Selected, with children** (???) - headers from this stream and any contained stream will be displayed in the list</li></ul>

## Important notes
* The processing of the file is done locally in your browser, using WebAssembly code. **No file content is sent to our servers**
* We still send some telemetry to help us understand the problem. Open browser's console to check the messages sent to our server.

## Feedback
Feel free to ask questions and share your thoughts about the app using GitHub issues. If you don't want others to see your message, contact us at analyzer@vtclab.com.

## Donate

* Bitcoin (BTC) Address: bc1qwt63dmhuyztlzpj6egu9s3tw052nl02653ymsf

* Ethereum (ETH) Address: 0x4A706ebcEdA0627A091e3CFa080C555e8561a288

* Patreon: https://www.patreon.com/vtclab_analyzer

## Version History
Quick summary about the changes between the versions is available [here](HISTORY.md)
