# Media Analyzer
The purpose of this repository is to provide a communication channel between the authors and the users of VTCLab Media Analyzer app (https://analyzer.vtclab.com)

In particular:
* To provide basic information about the application features and updates
* To gather feedback from the users (questions, problems, etc.)
* To discuss the ideas and upcoming changes

Currently, analyzer is in the "Private Alpha" stage, but you can request early access, send us a message at analyzer@vtclab.com.

### Contents
 
[Important notes](#important-notes)  
[Basic features](#basic-features)   
[Feedback](#feedback)    
[Donate](#donate)  
[Screenshots](#screenshots)

## Important notes
* The processing of the file is done locally in your browser. **No file content is sent to our servers**
* We still send some telemetry to help us understand the problem if any

## Basic features

|Containers supported|Comments|
| --- | --- |
| MPEG-TS | Parsing of TS packets, PAT/PMT & several other tables, PES packets and elementary streams inside them (if corresponding encoding is supported, see below), some descriptors |
| ISOFF / MP4 / MOV / QuickTime| Parsing of atom/box structure, display the contents of some known atoms/boxes. No parsing for 'mdat' yet. |
| Elementary | Most of the audio/video streams listed below are also supported as elementary streams |
| | |
| **Audio streams supported** |  |
| MPEG-1 Audio (ISO/IEC 11172-3)| Frame headers |
| MPEG-2 Audio (ISO/IEC 13818-3)| Frame headers |
| AAC Audio (ISO/IEC 13818-7, 14496-3), ADTS syntax| Frame headers |
| Dolby AC-3, E-AC-3 (ATSC A/52)| Frame headers |
| SMPTE-302M Audio | Frame headers |
| | |
| **Video streams supported** | |
| MPEG-1 Video (ISO/IEC 11172-2) | All headers except slice data and below |
| MPEG-2 Video (ISO/IEC 13818-2) | All headers except slice data and below |
| H.264/AVC Video | Location and types of NAL units, without much details |
| H.265/HEVC Video | Location and types of NAL units, without much details |
| H.266/VVC Video | Location and types of NAL units, without much details |
| | |
| **Common abilities** | |
| Packet filtering | Each stream has three-state mode selector: <ul><li>**Not selected** (✘) - headers from this stream won't be displayed in the list</li><li>**Selected, this stream only** (➔) - headers will be displayed, without contained streams</li><li>**Selected, with children** (✔) - headers from this stream and any contained stream will be displayed in the list</li></ul>

## Feedback
Feel free to ask questions and share your thoughts about the app using GitHub issues. If you don't want others to see your message, contact us at analyzer@vtclab.com.

## Donate

* Bitcoin (BTC) Address: bc1qwt63dmhuyztlzpj6egu9s3tw052nl02653ymsf

* Ethereum (ETH) Address: 0x4A706ebcEdA0627A091e3CFa080C555e8561a288

* Patreon: https://www.patreon.com/vtclab_analyzer

## Screenshots

<img width="1434" alt="Screenshot 1" src="https://user-images.githubusercontent.com/87360808/212826742-b8f7306e-fe32-4e9d-8566-ec3e51f5602d.png">
<img width="1435" alt="Screenshot 2" src="https://user-images.githubusercontent.com/87360808/212827399-aeb04aed-f8c8-4894-997b-a33fdb653085.png">
