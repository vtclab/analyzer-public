# Version History

## 2024-11-17 v0.5.6
* MP4: Google's spatial media boxes (spatial audio + spherical video)
* MP4: Support for some boxes common for HEIC files
* MP4: 'elng', 'iods', 'prft' boxes support
* MP4: ES_ID_Inc, ES_ID_Ref descriptors support
* MP4: `seig` group description support
* MP4: Read descriptors for several streams defined in ISO/IEC 14496-14 ("odsm", "crsm", "sdsm", "m7sm", "ocsm", "ipsm", "mjsm")
* MPEG-TS: Parse the contents of IOD_descriptor
* MPEG-1/2 audio: ID3 parsing support
* AVC: Print video dimensions

## 2024-07-28 v0.5.5
* MPEG-H audio support
* AVCHD LPCM audio support
* Parse Dolby RPU data in AV1 streams
* ST2094-40 metadata parsing
* Chinese HDR dynamic metadata support (T/UWA 005.1-2022)
* Recognize DJI 'meta' and 'dbgi' streams
* Fix network files processing

## 2024-06-08 v0.5.4
* Improve file type detection
* MPEG-TS: Improve PSI tables detection
* MP4/MOV: Add 'esds' box handling
* AC4: fix sync checking
* Small fixes for problems discovered by fuzzing

## 2024-05-08 v0.5.3
* HDMV PGS subtitles support
* Display TTML subtitle headers
* Recognize Teletext stream
* HEVC: sps_scc_extension, sps_3d_extension, sps_range_extension parsing
* MP4/MOV: Apple's stereo boxes description based on https://blog.mikeswanson.com/spatial
* SL-HDR SEI message support
* MPEG-TS: Add carousel_identifier_descriptor, association_tag_descriptor, deferred_association_tags_descriptor, T2_delivery_system_descriptor, target_region_descriptor, target_region_name_descriptor, URI_linkage_descriptor, related_content_descriptor, dvb_j_application_descriptor, dvb_j_application_location_descriptor support
* Display unknown PES data chunks
* SEI: MDPM data description
* MPEG-TS: Improve PSI sections detection
* DVB Subtitles: Fix alternative CLUT reading

## 2024-04-05 v0.5.2
* Add AVS2/AVS3 video support
* AVI subtitles support
* IVF format support
* Recognize AV1 in elementary OBU files
* Recognize VP8/VP9 video in MP4 containers
* PES: extended_stream_id handling
* MPEG-TS: DVB content_identifier_descriptor support
* Add dark theme & theme switching
* VP8: Fix width & height calculation

## 2024-03-14 v0.5.1
* Add DVB subtitles support
* Add SCTE-27 subtitles support
* Add drop-down menus for main UI panels
* mpegts: Fix first PSI section parsing if pointer_field is not zero
* mpegts: Fix error reporting for PSI tables with no stuffing

## 2024-02-22 v0.5.0
* Major UI rework (dockable panels, command palette, hex view, context menus)
* Search bytes/strings in the packet names or hex view
* MP4: Add box names/structure from "Apple HEVC Stereo Video Format additions"
* Print PES details (PTS/DTS/... presence) in the packet name
* Print TS details (adaptation_field/payload_unit_start/PCR/OPCR/... presence, TS PID) in the packet name
* Fix st2094_10 user data reading with ext_block_level == 2
* MP4: Add "rtmd" box name/recognition
* TS: Add S2_satellite_delivery_system_descriptor support
* RIFF: names for OpenDML chunks
* MKV: Fix reading of AVC/HEVC/VVC decoder configs
* AVC: Improve dec_ref_pic_marking_repetition parsing
* Extend number of known GUIDs in WAVE_FORMAT_EXTENSIBLE
* Recognize more video formats from VIDEOINFOHEADER


## 2024-01-05 v0.4.3
* VVC: support Picture Header parsing, improved PPS parsing
* MP4: update box names and sample entry names from ISO/IEC 14496-15
* MP4: support 'sync' and 'tscl' group description entries
* RIFF: add OpenDML AVI headers support
* AVI/MKV: print extra data in BITMAPINFOHEADER (if any)
* MPEG-TS: fix default_authority_descriptor parsing
* RIFF: fix stream assignment

## 2023-12-08 v0.4.2
* Support LOAS/LATM AAC wrapping
* Add FLAC audio support
* AV1: support 'metadata_obu'
* AAC: parse the beginning of AAC RAW packet
* Display 'sei_message' types in the header name for AVC/HEVC/VVC streams
* Recognize AnnexB streams stored in MP4 containers
* Improve streams detection algorithm
* More field descriptions for MPEG 1/2 Audio, AAC, AC-3 headers, MPEG-TS descriptors
* MPEG-TS: Support DVB 'message_descriptor', "metadata_pointer_descriptor", 'TTML_subtitling_descriptor'
* AVC: support 'frame_packing_assignment' SEI
* If (only) the type of the stream is known, display it as "Unknown Video", "Unknown Audio", etc
* MP4: Improve progress reporting for fragmented files
* ProRes: Fix parsing of interlaced streams

## 2023-11-15 v0.4.1
* Support 'spatial video' files shot by iPhone 15 Pro
* HEVC: parse 'three_dimensional_reference_displays_info' SEI, multilayer version of SPS, 'sps_multilayer_extension', 'pps_multilayer_extension' structures
* MP4/MOV: Support 'lhvC' box
* Visualization: show slice_type and layer_id (if not 0) in the header name for AVC/HEVC/VVC streams

## 2023-11-07 v0.4.0
* VP8, VP9, AV1 video streams parsing
* New formats supported: AVI, WAV, FLV
* Fragmented MP4 files support
* Extend parsing of AC-4 streams
* Display Dolby Vision RPU data headers
* Improve streams recognition, parsing performance
* Various fixes for problems discovered by fuzzy testing
* MP4: support 'chnl', 'albm', 'yrrc', 'loci', 'hnti', 'hinf' boxes
* More descriptions for AC-4, AC-4, MPEG 1/2 Video, AVC and HEVC elements
* Visualization: if raw bytes looks like a text, display them as a text


## 2023-10-03 v0.3.0
* Matroska (MKV), WebM files support
* MP4: Add 'styp', 'saiz', 'saio', 'pssh', 'tenc','trep', 'dfLa', 'cslg', 'stps', 'sdtp' boxes support
* MP4: Display track references info ('tref' box)
* MP4: Display raw data chunks for some unsupported codecs
* SEI: ST2094-10 data, film_grain_characteristics, alpha_channel_info support
* SEI: Add support of AVCIntra data sei
* Improve streams recognition
* MP4: rework handling of NAL-based streams
* MP4: Improve performance of raw streams extraction, when there are a lot of small samples
* MP4: Display names for metadata items as numbered list
* MP4: Fix Timecode reading
* PES: Fix usage of tref_extension_flag
* HEVC: Fix crash on invalid array read
* RBSP: Fix corner case on reading
* MP4: Fix 'File Info' binding
* AVC: Fix mvc_vui_parameters_extension reading

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
