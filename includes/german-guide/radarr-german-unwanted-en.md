<!-- markdownlint-disable MD041-->
??? abstract "German Unwanted - [Click to show/hide]"

    | Custom Format                                                                                                                       |                                      Score                                      | Trash ID                                                  |
    | ----------------------------------------------------------------------------------------------------------------------------------- | :-----------------------------------------------------------------------------: | --------------------------------------------------------- |
    | [{{ radarr['cf']['br-disk']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#br-disk)                                       |             {{ radarr['cf']['br-disk']['trash_scores']['german'] }}             | {{ radarr['cf']['br-disk']['trash_id'] }}                 |
    | [{{ radarr['cf']['generated-dynamic-hdr']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#generated-dynamic-hdr) :warning: | :warning: {{ radarr['cf']['generated-dynamic-hdr']['trash_scores']['german'] }} | {{ radarr['cf']['generated-dynamic-hdr']['trash_id'] }}   |
    | [{{ radarr['cf']['3d']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#3d)                                                 |               {{ radarr['cf']['3d']['trash_scores']['german'] }}                | {{ radarr['cf']['3d']['trash_id'] }}                      |
    | [{{ radarr['cf']['line-mic-dubbed']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#linemic-dubbed)                        |         {{ radarr['cf']['line-mic-dubbed']['trash_scores']['german'] }}         | {{ radarr['cf']['line-mic-dubbed']['trash_id'] }}         |
    | [{{ radarr['cf']['lq']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#lq)                                                 |               {{ radarr['cf']['lq']['trash_scores']['german'] }}                | {{ radarr['cf']['lq']['trash_id'] }}                      |
    | [{{ radarr['cf']['lq-release-title']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#lq-release-title)                     |        {{ radarr['cf']['lq-release-title']['trash_scores']['german'] }}         | {{ radarr['cf']['lq-release-title']['trash_id'] }}        |
    | [{{ radarr['cf']['german-lq']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#german-lq)                                   |           {{ radarr['cf']['german-lq']['trash_scores']['default'] }}            | {{ radarr['cf']['german-lq']['trash_id'] }}               |
    | [{{ radarr['cf']['german-lq-release-title']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#german-lq-release-title)       |    {{ radarr['cf']['german-lq-release-title']['trash_scores']['default'] }}     | {{ radarr['cf']['german-lq-release-title']['trash_id'] }} |
    | [{{ radarr['cf']['german-microsized']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#german-microsized)                   |       {{ radarr['cf']['german-microsized']['trash_scores']['default'] }}        | {{ radarr['cf']['german-microsized']['trash_id'] }}       |
    | [{{ radarr['cf']['x265-hd']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#x265-hd) :warning:                             |        :warning: {{ radarr['cf']['x265-hd']['trash_scores']['german'] }}        | {{ radarr['cf']['x265-hd']['trash_id'] }}                 |
    | [{{ radarr['cf']['extras']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#extras)                                         |             {{ radarr['cf']['extras']['trash_scores']['german'] }}              | {{ radarr['cf']['extras']['trash_id'] }}                  |
    | [{{ radarr['cf']['av1']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#av1)                                               |               {{ radarr['cf']['av1']['trash_scores']['german'] }}               | {{ radarr['cf']['av1']['trash_id'] }}                     |
    | [{{ radarr['cf']['upscaled']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#upscaled)                                     |            {{ radarr['cf']['upscaled']['trash_scores']['german'] }}             | {{ radarr['cf']['upscaled']['trash_id'] }}                |

    ---

    Breakdown and Why

    - **{{ radarr['cf']['br-disk']['name'] }}:** This is a custom format to help Radarr recognize & ignore BR-DISK (ISO's and Blu-ray folder structure) in addition to the standard BR-DISK quality.
    - :warning: **{{ radarr['cf']['generated-dynamic-hdr']['name'] }}:** A collection of groups known to generate their own dynamic HDR metadata - Dolby Vision and/or HDR10+. At least one German group (VECTOR) generally provides good-quality releases but creates (subjectively better) Generated Dynamic HDR for some. If you don't care about Generated Dynamic HDR and/or don't want to avoid VECTOR releases, set this score to `0`. If you're going to prevent Generated Dynamic HDR set this score to `-10000`.
    - **{{ radarr['cf']['3d']['name'] }}:** Is 3D still a thing for home use ?
    - **{{ radarr['cf']['line-mic-dubbed']['name'] }}:** This blocks Line and Mic Dubs.
    - **{{ radarr['cf']['lq']['name'] }}:** A collection of known Low Quality groups that are often banned from the the top trackers because the lack of quality or other reasons.
    - **{{ radarr['cf']['lq-release-title']['name'] }}:** A collection of terms seen in the titles of low-quality releases that are not captured by using a release group name.
    - **{{ radarr['cf']['german-lq']['name'] }}:** A collection of known Low Quality German groups that are often banned from the the top trackers because the lack of quality or other reasons.
    - **{{ radarr['cf']['german-lq-release-title']['name'] }}:** A collection of terms seen in the titles of low-quality releases that are not captured by using a release group name.
    - **{{ radarr['cf']['german-microsized']['name'] }}:** A collection of German groups producing low quality micro-sized releases.
    - :warning: **{{ radarr['cf']['x265-hd']['name'] }}:** This blocks/ignores 720/1080p (HD) releases that are encoded in x265. However as there are certain german groups (ZeroTwo, VECTOR, ...) which produce high bitrate 1080p x265 encodes we recommend setting the score of this custom format to 0.
    - **{{ radarr['cf']['extras']['name'] }}:** Blocks releases that only contain extras
    - **{{ radarr['cf']['av1']['name'] }}:** This blocks all releases encoded in AV1.
    - **{{ radarr['cf']['upscaled']['name'] }}:** A custom format to prevent Radarr from grabbing upscaled releases.
<!-- markdownlint-enable MD041-->
