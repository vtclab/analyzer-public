# Support for various frames

## Support levels
| Level | Meaning |
| --- | --- |
| 1 | Not supported |
| 2 | Only some properties are supported |
| 3 | All properties are supported, without describing the values |
| 4 | All properties are supported, with description of some values |
| 5 | All properties are supported, with description of all values |

## MPEG-TS
|  | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- |
| TS Packet |  |  |  |  | &#10004; |
| adaptation_field |  |  |  | &#10004; |  |
| adaptation_field_extension |  |  |  | &#10004; |  |
| af_descriptor | &#10004; |  |  |  |  |
| **PSI Tables (MPEG)** |  |  |  |  |  |
| Program Association Table |  |  |  |  | &#10004; |
| Conditional Access Table |  |  |  |  | &#10004; |
| Program Map Table |  |  |  |  | &#10004; |
| TS Description Table |  |  |  |  | &#10004; |
| **PSI Tables (DVB)** |  |  |  |  |  |
| Network Information Table |  |  |  |  | &#10004; |
| Service Description Table |  |  | &#10004; |  |  |
| Bouquet Association Table |  |  |  |  | &#10004; |
| Event Information Table |  |  |  | &#10004; |  |
| Time Date Table |  |  |  |  | &#10004; |
| Running Status Table |  |  | &#10004; |  |  |
| Stuffing Table |  |  |  |  | &#10004; |
| Time Offset Table |  |  |  |  | &#10004; |
| Application Information Table |  |  | &#10004; |  |  |
| Discontinuity Information Table |  |  |  |  | &#10004; |
| Selection Information Table |  |  | &#10004; |  |  |
| **Descriptors (MPEG)** |  |  |  |  |  |
| video_stream_descriptor |  |  | &#10004; |  |  |
| audio_stream_descriptor |  |  | &#10004; |  |  |
| hierarchy_descriptor |  |  | &#10004; |  |  |
| registration_descriptor |  |  |  |  | &#10004; |
| data_stream_alignment_descriptor |  |  | &#10004; |  |  |
| target_background_grid_descriptor |  |  | &#10004; |  |  |
| video_window_descriptor |  |  |  |  | &#10004; |
| CA_descriptor |  |  | &#10004; |  |  |
| copyright_descriptor |  |  | &#10004; |  |  |
| maximum_bitrate_descriptor |  |  | &#10004; |  |  |
| private_data_indicator_descriptor |  |  | &#10004; |  |  |
| smoothing_buffer_descriptor |  |  | &#10004; |  |  |
| STD_descriptor |  |  |  |  | &#10004; |
| IBP_descriptor |  |  |  |  | &#10004; |
| ISO_639_language_descriptor |  |  |  |  | &#10004; |
| system_clock_descriptor |  |  |  |  | &#10004; |
| multiplex_buffer_utilization_descriptor |  |  |  |  | &#10004; |
| AVC video descriptor |  |  |  |  | &#10004; |
| AVC timing and HRD descriptor |  |  |  |  | &#10004; |
| mpeg2_aac_audio_descriptor |  |  |  |  | &#10004; |
| J2K video descriptor |  |  |  |  | &#10004; |
| HEVC video descriptor |  |  |  |  | &#10004; |
| **Descriptors (DVB)** |  |  |  |  |  |
| network_name_descriptor |  |  |  |  | &#10004; |
| service_list_descriptor |  |  | &#10004; |  |  |
| stuffing_descriptor |  |  |  |  | &#10004; |
| satellite_delivery_system_descriptor |  |  | &#10004; |  |  |
| cable_delivery_system_descriptor |  |  | &#10004; |  |  |
| VBI_data_descriptor |  |  | &#10004; |  |  |
| VBI_teletext_descriptor |  |  |  | &#10004; |  |
| bouquet_name_descriptor |  |  |  |  | &#10004; |
| service_descriptor |  |  |  | &#10004; |  |
| country_availability_descriptor |  |  |  |  | &#10004; |
| linkage_descriptor |  | &#10004; |  |  |  |
| NVOD_reference_descriptor |  |  |  |  | &#10004; |
| time_shifted_service_descriptor |  |  |  |  | &#10004; |
| short_event_descriptor |  |  |  |  | &#10004; |
| extended_event_descriptor |  |  |  |  | &#10004; |
| time_shifted_event_descriptor |  |  |  |  | &#10004; |
| component_descriptor |  |  |  | &#10004; |  |
| mosaic_descriptor |  | &#10004; |  |  |  |
| stream_identifier_descriptor |  |  |  |  | &#10004; |
| CA_identifier_descriptor |  |  | &#10004; |  |  |
| content_descriptor |  |  | &#10004; |  |  |
| parental_rating_descriptor |  |  |  | &#10004; |  |
| teletext_descriptor |  |  |  | &#10004; |  |
| telephone_descriptor |  |  |  | &#10004; |  |
| local_time_offset_descriptor |  |  |  | &#10004; |  |
| subtitling_descriptor |  |  |  | &#10004; |  |
| terrestrial_delivery_system_descriptor |  |  | &#10004; |  |  |
| multilingual_network_name_descriptor |  |  |  |  | &#10004; |
| multilingual_bouquet_name_descriptor |  |  |  |  | &#10004; |
| multilingual_service_name_descriptor |  |  |  |  | &#10004; |
| multilingual_component_descriptor |  |  |  |  | &#10004; |
| private_data_specifier_descriptor |  |  | &#10004; |  |  |
| service_move_descriptor |  |  |  |  | &#10004; |
| short_smoothing_buffer_descriptor|  |  | &#10004; |  |  |
| frequency_list_descriptor |  |  | &#10004; |  |  |
| partial_transport_stream_descriptor |  |  | &#10004; |  |  |
| data_broadcast_descriptor |  |  |  | &#10004; |  |
| scrambling_descriptor |  |  | &#10004; |  |  |
| data_broadcast_id_descriptor |  |  | &#10004; |  |  |
| transport_stream_descriptor |  |  |  |  | &#10004; |
| DSNG_descriptor |  |  |  |  | &#10004; |
| PDC_descriptor |  |  | &#10004; |  |  |
| AC-3_descriptor |  |  | &#10004; |  |  |
| ancillary_data_descriptor |  |  | &#10004; |  |  |
| cell_list_descriptor | &#10004; |  |  |  |  |
| cell_frequency_link_descriptor | &#10004; |  |  |  |  |
| announcement_support_descriptor |  | &#10004; |  |  |  |
| application_signalling_descriptor | &#10004; |  |  |  |  |
| adaptation_field_data_descriptor |  |  | &#10004; |  |  |
| service_identifier_descriptor | &#10004; |  |  |  |  |
| service_availability_descriptor |  |  | &#10004; |  |  |
| default_authority_descriptor |  |  | &#10004; |  |  |
| related_content_descriptor | &#10004; |  |  |  |  |
| TVA_id_descriptor | &#10004; |  |  |  |  |
| content_identifier_descriptor | &#10004; |  |  |  |  |
| time_slice_fec_identifier_descriptor | &#10004; |  |  |  |  |
| ECM_repetition_rate_descriptor | &#10004; |  |  |  |  |
| S2_satellite_delivery_system_descriptor | &#10004; |  |  |  |  |
| enhanced_AC-3_descriptor |  |  | &#10004; |  |  |
| DTS_descriptor |  |  | &#10004; |  |  |
| AAC_descriptor |  |  | &#10004; |  |  |
| XAIT_location_descriptor |  |  | &#10004; |  |  |
| FTA_content_management_descriptor |  |  | &#10004; |  |  |
| supplementary_audio_descriptor |  |  |  | &#10004; |  |
| AC-4_descriptor |  |  | &#10004; |  |  |
| DTS-HD_descriptor | &#10004; |  |  |  |  |
| TTML_subtitling_descriptor | &#10004; |  |  |  |  |
| DTS-UHD_descriptor | &#10004; |  |  |  |  |
| **Descriptors (DVB, Multimedia Home Platform)** |  |  |  |  |  |
| application_descriptor |  |  | &#10004; |  |  |
| application_name_descriptor |  |  |  |  | &#10004; |
| transport_protocol_descriptor | &#10004; |  |  |  |  |
| dvb_j_application_descriptor | &#10004; |  |  |  |  |
| dvb_j_application_location_descriptor | &#10004; |  |  |  |  |
| sexternal_application_authorization_descriptor |  |  | &#10004; |  |  |
| dvb_html_application_descriptor | &#10004; |  |  |  |  |
| dvb_html_application_location_descriptor | &#10004; |  |  |  |  |
| dvb_html_application_boundary_descriptor | &#10004; |  |  |  |  |
| application_icons_descriptor |  |  | &#10004; |  |  |
| prefetch_descriptor | &#10004; |  |  |  |  |
| DII_location_descriptor | &#10004; |  |  |  |  |
| delegated_application_descriptor | &#10004; |  |  |  |  |
| plug-in_descriptor | &#10004; |  |  |  |  |
| application_storage_descriptor | &#10004; |  |  |  |  |
| ip_signalling_descriptor | &#10004; |  |  |  |  |
| provider_export_descriptor | &#10004; |  |  |  |  |
| provider_usage_descriptor | &#10004; |  |  |  |  |
| graphics_constraints_descriptor | &#10004; |  |  |  |  |
| private_data_specifier_descriptor | &#10004; |  |  |  |  |
| **Descriptors (ATSC)** |  |  |  |  |  |
| AC-3_audio_stream_descriptor |  |  |  | &#10004; |  |
| E-AC-3_audio_descriptor |  |  |  | &#10004; |  |

## MP4/MOV

|  | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- |
| "ftyp" |  |  |  |  | &#10004; |
| "mvhd" |  |  |  | &#10004; |  |
| "vmhd" |  |  |  | &#10004; |  |
| "tkhd" |  |  |  | &#10004; |  |
| "mdhd" |  |  |  | &#10004; |  |
| "hdlr" |  |  |  |  | &#10004; |
| "elst" |  |  | &#10004; |  |  |
| "dref" |  |  |  |  | &#10004; |
| "smhd" |  |  | &#10004; |  |  |
| "stsd" |  |  |  |  | &#10004; |
| "stts" |  |  |  |  | &#10004; |
| "ctts" |  |  |  |  | &#10004; |
| "stsc" |  |  |  |  | &#10004; |
| "stco" |  |  |  |  | &#10004; |
| "co64" |  |  |  |  | &#10004; |
| "stsz" |  |  |  |  | &#10004; |
| "esds" |  |  | &#10004; |  |  |
| "url " |  |  |  |  | &#10004; |
| "urn " |  |  |  |  | &#10004; |
| "imdt" |  |  | &#10004; |  |  |
| "snim" |  |  |  |  | &#10004; |
| "colr" |  |  | &#10004; |  |  |
| "pasp" |  |  | &#10004; |  |  |
| "clap" |  |  | &#10004; |  |  |
| "fiel" |  |  | &#10004; |  |  |
| "frma" |  |  |  |  | &#10004; |
| "chan" |  |  | &#10004; |  |  |
| "clef" |  |  |  |  | &#10004; |
| "prof" |  |  |  |  | &#10004; |
| "enof" |  |  |  |  | &#10004; |
| "avcC" |  |  | &#10004; |  |  |
| "moov" |  |  |  |  | &#10004; |
| "trak" |  |  |  |  | &#10004; |
| "trgr" |  |  |  |  | &#10004; |
| "mdia" |  |  |  |  | &#10004; |
| "minf" |  |  |  |  | &#10004; |
| "stbl" |  |  |  |  | &#10004; |
| "edts" |  |  |  |  | &#10004; |
| "dinf" |  |  |  |  | &#10004; |
| "udta" |  |  |  |  | &#10004; |
| "strd" |  |  |  |  | &#10004; |
| "grpl" |  |  |  |  | &#10004; |
| "hnti" |  |  |  |  | &#10004; |
| "hinf" |  |  |  |  | &#10004; |
| "mvex" |  |  |  |  | &#10004; |
| "moof" |  |  |  |  | &#10004; |
| "traf" |  |  |  |  | &#10004; |
| "mfra" |  |  |  |  | &#10004; |
| "strk" |  |  |  |  | &#10004; |
| "otyp" |  |  |  |  | &#10004; |
| "setu" |  |  |  |  | &#10004; |
| "wave" |  |  |  |  | &#10004; |
| "tapt" |  |  |  |  | &#10004; |
