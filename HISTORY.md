# Version History

## 2023-09-04 v0.2.6
* Add support of Timed Text ('tx3g', 'text' sample entries) in MP4/MOV files
* Add basic handling of  AC-4 streams ('ac4_syncframe' only) in MP4 & TS files
* MPEG-TS: Support PSI tables & descriptors from ATSC A/65 standard, recognize all descriptors listed in DVB BlueBook A038r16
* Add descriptions for 'cc_type' 'active_format', 'video_format' fields
* Include PES packet type ('audio', 'video', private') to header name
* Add basic detection of MPEG Program / System Streams
* MP4/MOV: recognize more 'udta' boxes
* Improve probe algorithm: better recognition of MP4, small TS files
* Fix freezing in some cases of H.264 parsing

## 2023-08-03 v0.2.5
* TS: SCTE-35 streams support (commands only, no descriptors yet)
* SEI: Add ATSC cc_data/bar_data/afd_data support in itu35 registered SEI
* MP4: Support various flavours of XDCAM (MPEG-2) video
* HEVC: time_code SEI support
* TS: MHP AIT transport_protocol_descriptor support
* Visualization: group long list of values into chunks of four items
* MP4: support simple 'udta' boxes from 3GPP spec
* MP4: Add 'av1C' (AV1CodecConfigurationBox), 'dOps' (OpusSpecificBox), 'dac4' (AC4SpecificBox) boxes support
* MP4: basic recognition of compressed movie atoms ('cmov', 'dcom', 'cmvd')
* Visualization: Print number of bytes in the utf8 string
* TS: fix tag&length display for MHP AIT descriptors
* MP4: fix hvcC flags display
* Fix tables and arrays visualization

## 2023-07-06 v0.2.4
* MP4: Support 'schm', 'sinf', 'schi', 'sgpd' 'sbgp', 'mehd', 'trex', 'sidx', 'mfhd', 'tfhd', 'tfdt', trun', 'mdcv', 'clli', 'cclv' boxes
* TS: Add new PMT stream_types and descriptors from ISO/IEC 13818-1:2022
* TS/MP4/AVC/HEVC/VVC: Add enum names for AspectRatio, ChromaFormat, ColourPrimaries, TransferCharacteristics, MatrixCoefficients and HDR_WCG_idc fields, human-friendly descriptions for luminance- and color-related fields
* TS: Add DOVI_video_stream_descriptor support
* TS: Recognise SCTE-35 streams, add 'cue_identifier_descriptor' support
* VVC: Add support for several SEI messages, list names for others
* VVC: APS header support, picture_header_structure draft
* HEVC: Add names for Dolby Vision "Unspecified 62" and "Unspecified 63" NAL units
* SEI: Add Kvazaar, Elemental info from SEI Unregistered messages
* RBSP reader for AVC/HEVC/VVC: Fix incorrect behavior in some corner cases

## 2023-06-05 v0.2.3
* Basic detection of RIFF (*.avi and *.wav), EBML (Matroska, WebM), MXF files
* QT timecode tracks support
* MVC-related boxes and NAL units
* QuickTime: basic support for mebx (QT "Timed metadata") atoms
* Scroll Jog control to be able to scroll the list with constant (adjustable) speed
* Navigation Bar: Support negative values of file position and item indexes
* SEI: Display x264, x265, ATEME info from SEI unregistered, recognize MDPM info presence
* AVC: Fix scaling list parsing
* RBSP: Fix incorrect data reading in some edge cases causing incorrect reading of some AVC/HEVC/VVC headers
* HEVC: Fix short-term ref pics set parsing

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
