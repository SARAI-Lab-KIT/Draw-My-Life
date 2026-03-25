# Extracted Features

All the extracted features, in aggregated format, can be found in the file [extracted_features_final.xlsx](https://github.com/SARAI-Lab-KIT/Draw-My-Life/blob/main/extracted_features/extracted_features_final.xlsx).

Below, you will find a list describing each extracted feature. The drawing dynamics features were extracted from the participants' drawing logs collected in real time by the tablet ROS2 node. The drawing production features were extracted from the final version of the participants' drawing. The speech dynamics features were extracted from the participants' cleaned audio recording. The speech production features were extracted from the participants' transcript.

| Feature                                  | Extracted from     |    Description  |
| :--------------------------------------: | :----------------: |:-------------: |
| activity_time                            | Drawing dynamics   | total time spent in the activity |
| total_stroke_count                       | Drawing dynamics   | total number of strokes produced |
| stroke_total_length                      | Drawing dynamics   | cumulative length of all strokes |
| stroke_mean_length                       | Drawing dynamics   | average length of strokes |
| stroke_std_length                        | Drawing dynamics   | variability in stroke lengths |
| stroke_mean_speed                        | Drawing dynamics   | average speed of strokes |
| stroke_std_speed                         | Drawing dynamics   | variability in stroke speed |
| stroke_mean_accel                        | Drawing dynamics   | average acceleration of strokes |
| stroke_std_accel                         | Drawing dynamics   | variability in stroke acceleration |
| stroke_mean_pressure                     | Drawing dynamics   | average pressure of strokes |
| stroke_std_pressure                      | Drawing dynamics   | variability in stroke pressure |
| stroke_pressure_slope                    | Drawing dynamics   | slope of pressure change over time |
| pen_size_used_count                      | Drawing dynamics   | number of distinct pen sizes used |
| pen_size_mean                            | Drawing dynamics   | average pen size of strokes |
| pen_size_std                             | Drawing dynamics   | variability in stroke pen size |
| stroke_mean_curvature                    | Drawing dynamics   | average curvature of strokes |
| stroke_mean_angularity                   | Drawing dynamics   | average sharpness/angle of strokes |
| avg_time_between_strokes                 | Drawing dynamics   | average time between strokes  |
| std_time_between_strokes                 | Drawing dynamics   | variability of inter-stroke intervals |
| total_pause_time                         | Drawing dynamics   | total inter-stroke intervals time |
| pause_ratio                              | Drawing dynamics   | ratio between total_pause_time and activity_time |
| stroke_frequency                         | Drawing dynamics   | rate of strokes over time |
| net_erased_pixels                        | Drawing dynamics   | total number of erased/undone pixels |
| undone_erased_stroke_count               | Drawing dynamics   | number of fully-erased or undone strokes |
| undone_erased_stroke_ratio               | Drawing dynamics   | ratio between undone_erased_stroke_count and total_stroke_count |
| surface_coverage_ratio                   | Drawing production | proportion of canvas area covered by drawing |
| pixel_std_x                              | Drawing production | horizontal dispersion of drawn pixels |
| pixel_std_y                              | Drawing production | vertical dispersion of drawn pixels |
| mean_distance_center                     | Drawing production | average distance of drawing elements from canvas center |
| left_right_balance                       | Drawing production | balance of content between left and right sides |
| top_bottom_balance                       | Drawing production | balance of content between top and bottom sides |
| colors_used_count                        | Drawing production | number of distinct colors used |
| mean_hue                                 | Drawing production | average hue value of colors used |
| std_hue                                  | Drawing production | variability in hue values |
| mean_saturation                          | Drawing production | average saturation of colors used |
| std_saturation                           | Drawing production | variability in saturation values |
| mean_brightness                          | Drawing production | average brightness of colors used |
| std_brightness                           | Drawing production | variability in brightness values |
| black_ratio                              | Drawing production | ratio between black pixels and non black pixels (excluding white background pixels) |
| warm_cool_ratio                          | Drawing production | ratio between warm pixels and cool pixels based on hue (excluding white background pixels)|
| drawing_human_presence                   | Drawing production | presence of human-related elements |
| drawing_object_presence                  | Drawing production | presence of objects |
| drawing_nature_animals_presence          | Drawing production | presence of nature or animal elements |
| drawing_emotional_symbols_presence       | Drawing production | presence of symbols conveying emotions |
| drawing_first_person_text_presence       | Drawing production | presence of first-person textual elements |
| drawing_abstract_shapes_presence         | Drawing production | presence of abstract shapes |
| F0semitoneFrom27.5Hz_sma3nz_amean        | Speech dynamics    | mean fundamental frequency (pitch) |
| F0semitoneFrom27.5Hz_sma3nz_stddevNorm   | Speech dynamics    | normalized variability of pitch |
| F0semitoneFrom27.5Hz_sma3nz_pctlrange0-2 | Speech dynamics    | pitch range between percentiles |
| loudness_sma3_amean                      | Speech dynamics    | average vocal loudness |
| loudness_sma3_stddevNorm                 | Speech dynamics    | variability of loudness |
| jitterLocal_sma3nz_amean                 | Speech dynamics    | cycle-to-cycle variation in fundamental frequency |
| shimmerLocaldB_sma3nz_amean              | Speech dynamics    | cycle-to-cycle variation in amplitude |
| HNRdBACF_sma3nz_amean                    | Speech dynamics    | harmonic-to-noise ratio of the voice signal |
| total_speech_time                        | Speech dynamics    | total duration of speech |
| speech_ratio                             | Speech dynamics    | ratio between total_speech_time and activity_time |
| word_count                               | Speech production  | total number of spoken words |
| mean_word_count_sentence                 | Speech production  | average number of words per sentence |
| word_count_per_sec                       | Speech production  | ratio between word_count and activity_time |
| hesitation_markers_ratio                 | Speech production  | ratio between number of hesitation markers and word_count |
| mattr                                    | Speech production  | measure of lexical diversity (Moving-Average Type-Token Ratio) |
| mean_disclosure_depth                    | Speech production  | transcript average self-disclosure depth |