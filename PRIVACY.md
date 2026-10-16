# TUKZFY Privacy Policy

**Application:** TUKZFY — Windows desktop music application  
**Developer:** Independent developer of TUKZFY  
**Effective date:** [INSERT PUBLICATION DATE]  
**Privacy contact:** [INSERT CONTACT EMAIL]

> **Publication checklist:** Replace the bracketed fields and verify the server-side statements before publishing. This policy describes the reviewed TUKZFY v18.12.17 desktop code; the separately hosted search service and any future versions require additional review.

## 1. Overview

TUKZFY is a Windows desktop application that helps users discover music-related videos and playlists and access eligible videos through an embedded YouTube player. It also displays artist information and images obtained from Deezer. This policy explains what information the desktop application processes, how third-party services are involved, and the choices available to users.

## 2. Information processed by TUKZFY

### 2.1 Search terms and search results

When you search, TUKZFY sends the search term and selected search type to its search service at `https://tukzfy-api.tukzhacker.workers.dev`. That service is used to retrieve video or playlist results from YouTube-related services. Search terms can reveal interests and preferences. **The operator must verify and document whether the search service logs IP addresses, search terms, timestamps, request metadata, or other information, and how long those logs are retained.**

The desktop application stores successful search responses in a local cache to reduce repeated requests. In the reviewed version, cache entries are eligible for reuse for seven days; this does **not** mean the files are automatically deleted after seven days. Old files may remain until removed by the user or application maintenance. The developer must review cache retention against applicable YouTube API policies.

### 2.2 Locally stored preferences and favorites

The reviewed desktop application stores certain information on your device, including favorite video identifiers, the last saved volume setting, and cached search results. This information is used to provide app features and restore preferences. The application may also maintain information in memory during a session, such as the current playback queue and artist images.

### 2.3 Artist searches and images

To display artist banners, TUKZFY requests artist information and images from Deezer (`api.deezer.com` and the image hosts returned by that service). The requested artist name and technical connection information may be received by those services under their own policies.

### 2.4 Video playback

TUKZFY uses an embedded YouTube player to display and play supported videos. YouTube and Google may receive video identifiers, IP addresses, device/browser information, cookies or similar technical data through the embedded player, subject to their own policies and settings. TUKZFY does not control the independent data processing performed by YouTube or Google.

### 2.5 Technical and diagnostic information

Network services can receive technical information needed to deliver requests, such as IP addresses and request headers. Whether the TUKZFY search service retains logs, analytics, or security records must be confirmed with its hosting configuration before publication. The reviewed desktop code alone is not sufficient to verify server-side logging practices.

## 3. Purposes of processing

Information is processed to perform searches requested by users, show video and playlist results, load the embedded player, display artist images, maintain playback preferences and favorites, improve responsiveness through local caching, and support service reliability and security where applicable.

## 4. Third-party services

TUKZFY integrates with third-party providers, which may independently process information:

- **YouTube / Google:** search-related data and embedded video playback. [Google Privacy Policy](https://policies.google.com/privacy) and [YouTube Terms of Service](https://www.youtube.com/t/terms).
- **Deezer:** artist lookup and images. [Deezer](https://www.deezer.com/).
- **Cloudflare:** the TUKZFY search service uses a `workers.dev` endpoint. Hosting infrastructure may process connection metadata. [Cloudflare Privacy Policy](https://www.cloudflare.com/privacypolicy/).
- **Instagram:** the application includes a link that opens an external Instagram page when selected. [Instagram Privacy Policy](https://privacycenter.instagram.com/policy/).

These services have their own terms and privacy practices. Links to third-party policies are provided for convenience; their content is controlled by those providers.

## 5. Sharing and sale of personal information

TUKZFY transmits information to the services needed to provide search, artist lookup, and playback as described above. **The developer must verify whether the hosted search service uses additional subprocessors, analytics, logs, or data sharing before making any broader claims that information is never shared, sold, or used for advertising.** The reviewed desktop code does not establish all server-side practices.

## 6. Storage and retention

Local application data is stored in the user's Windows profile, including files under `%LOCALAPPDATA%\TUKZFY`. Search-cache entries are reused for up to seven days in the reviewed version, but cache files may remain on disk beyond that period. Favorites and saved volume settings can remain until deleted or reset. Session-only artist images are kept in memory while the application runs.

Server-side log retention, if any, is **pending verification**. This policy must be updated with an accurate retention period or clear retention criteria before it is published as final.

## 7. Your choices and rights

You may stop using TUKZFY at any time. You can remove locally stored application data by closing TUKZFY and deleting its data folder under `%LOCALAPPDATA%\TUKZFY`; doing so may remove favorites, cached searches, and preferences. Uninstalling the application may not automatically delete all user data.

To request information about, correction of, or deletion of any data held by the developer or the hosted search service, contact **[INSERT CONTACT EMAIL]**. The developer will assess requests under applicable privacy law, including Brazil's LGPD where applicable. Requests concerning information held independently by Google, YouTube, Deezer, or Cloudflare may need to be directed to those providers.

## 8. Security

TUKZFY uses HTTPS endpoints for the reviewed search and third-party service requests. No internet-connected service can guarantee absolute security. The developer should restrict access to API credentials, keep dependencies updated, and review hosted-service access and retention settings. This policy does not claim an independent security certification or audit.

## 9. Children's privacy

TUKZFY is not specifically designed or marketed to children. The developer should establish an appropriate minimum age or parental-consent process if the application is offered to minors, in line with applicable laws and platform requirements. Do not include a claim that children are never users unless that can be supported.

## 10. International processing

The third-party services used by TUKZFY may process data in countries outside the user's country of residence. Applicable safeguards and rights depend on the service provider and relevant law.

## 11. YouTube API disclosures

TUKZFY uses YouTube API Services and an embedded YouTube player. By using YouTube functionality, users are also subject to the [YouTube Terms of Service](https://www.youtube.com/t/terms) and [Google Privacy Policy](https://policies.google.com/privacy). The developer must independently verify compliance with current [YouTube API Services Terms](https://developers.google.com/youtube/terms/api-services-terms-of-service) and related policies, including any rules governing storage, attribution, playback, and user-facing disclosures.

## 12. Changes to this policy

This policy may be updated when TUKZFY's functionality, third-party integrations, data handling, or legal requirements change. The effective date above will be updated when a revised version is published. Material changes should be communicated in an appropriate manner.

## 13. Contact

For privacy questions or requests concerning TUKZFY, contact:

**TUKZFY developer**  
**Email:** [INSERT CONTACT EMAIL]  
**Project:** https://github.com/tukzhacker-lab/TUKZFY-MUSIC
