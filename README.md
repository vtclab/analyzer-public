# Media Analyzer
The purpose of this repository is to provide a communication channel between the authors and the users of VTCLab Media Analyzer app (https://media-analyzer.pro)

In particular:
* To provide basic information about the application features and updates
* To gather feedback from the users (questions, problems, etc.)
* To discuss the ideas and upcoming changes

If you spot some issue which you are interested in, please vote for it with some emoji or comment.

Currently, analyzer is in the "Public Beta" stage, so don't be surprised if you spot something weird. If you do though, please, send us a message at analyzer@vtclab.com or open an issue here on GitHub.

### Contents
 
[Screenshots](#screenshots)     
[Basic features](#basic-features)    
[Important notes](#important-notes)   
[Feedback](#feedback)     
[Donate](#donate)   
[Version history](#version-history)

## Screenshots

<a href="https://github.com/vtclab/analyzer-public/assets/87360808/7b27c42d-8890-4747-88f6-a4d5bc1bb694"><img width="100" alt="Screenshot 1" src="https://github.com/vtclab/analyzer-public/assets/87360808/7b27c42d-8890-4747-88f6-a4d5bc1bb694"></a>
<a href="https://github.com/vtclab/analyzer-public/assets/87360808/b16049ac-4d9a-42f5-bc5b-fa7268c3043c"><img width="100" alt="Screenshot 2" src="https://github.com/vtclab/analyzer-public/assets/87360808/b16049ac-4d9a-42f5-bc5b-fa7268c3043c"></a>
<a href="https://github.com/vtclab/analyzer-public/assets/87360808/4d6bded9-37d9-41d3-8b4f-a5189ecdfa4b"><img width="100" alt="Screenshot 3" src="https://github.com/vtclab/analyzer-public/assets/87360808/4d6bded9-37d9-41d3-8b4f-a5189ecdfa4b"></a>

## Basic features

| **Supported** | |
| --- | --- |
| Containers | MPEG-TS, ISOFF / MP4 / 3GPP / MOV / QuickTime, MKV / WebM, RIFF / AVI / WAV, FLV, Elementary
| Video Codecs | MPEG-1 Video, MPEG-2 Video, H.264/AVC, H.265/HEVC Video, H.266/VVC, VP8, VP9, AV1, Apple ProRes, Dolby Vision RPU
Audio Codecs | MPEG-1 Audio, MPEG-2 Audio, AAC, Dolby AC-3, E-AC-3, AC-4, SMPTE-302M Audio  |
Subtitles | ISOBMFF Timed Text, DVB Subtitles, SCTE-27 Subtitles
Metadata | ATSC Service Information, DVB Service Information, Closed Captions, AFD, Bar data, ST2094-10 data, AVC / HEVC / VVC SEI messages, SCTE-35 data
| | |
| **Common abilities** | |
| Packet filtering | Each stream has three-state mode selector: <ul><li>**Not selected** (✘) - headers from this stream won't be displayed in the list</li><li>**Selected, this stream only** (➔) - headers will be displayed, without contained streams</li><li>**Selected, with children** (✔) - headers from this stream and any contained stream will be displayed in the list</li></ul>

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
