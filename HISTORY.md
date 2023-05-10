# Version History

## 2023-05-05 v0.2.2
* Add packet list navigator ("Go to header index", "Go to file position" commands)
* Improve packet list rendering for Firefox and Safari browsers
* MP4/MOV: Add 'meta', 'ilst' boxes support
* MP4/MOV: Fix DoviConfigurationBox ('dvcC') parsing 
* MP4/MOV: Extend the list sample entry names
* MP4/MOV: Support 'btrt' box
* AC-3: Support headers with bsid < 8
* Fix UUID visualization
* Improve packet caching

## 2023-04-04, v0.2.1
* MP4/MOV: Add support for ProRes, AC-3, E-AC-3 streams, raw video and audio chunks
* MP4/MOV: Add support for DolbyVision boxes
* MP4/MOV: Fix AAC Raw packet size displayed
* MP4/MOV: Display timecode sample entry contents
* HEVC: Add 'decoded_picture_hash' SEI
* HEVC, VVC: Fix stream displayed name
* More detailed error messages
* Add 'details' page
* Visual improvements

## 2023-03-10, v0.2.0, Public Beta
* MP4/MOV 'mdat' parsing for AAC/AVC/HEVC/VVC streams
* Advanced header parsing for AVC & HEVC, more details for VVC
* Many DVB descriptors and PSI tables added
* Visual improvements
* Performance improvements
* Stability improvements

## 2023-01-17, v0.1.0, Private Alpha

* Multiplexing Formats: MPEG-TS, MP4/MOV (basic atoms)
* Video Encodings: MPEG 1/2 Video (headers + details), AVC/HEVC/VVC (NAL Unit locations)
* Audio Encodings: MPEG 1/2 Audio, AAC, AC3, E-AC3 (headers + details)
* Packet filtering (by streams)
