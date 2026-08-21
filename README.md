<div align="center">

# Anton Smedberg

**iOS Developer** · Swift · SwiftUI · Swift Concurrency · Metal · AVFoundation

Malmö · Lund · Öresund · Greater Copenhagen — on-site, hybrid or remote

[Portfolio](https://antonsmedberg.github.io/) · [LinkedIn](https://www.linkedin.com/in/anton-smedberg-a9aa6121b/) · [anton@smedberg.eu](mailto:anton@smedberg.eu)

</div>

I build native iOS apps in Swift and SwiftUI. Most of my work sits where concurrency meets media and system frameworks: `async/await` and actors under Swift 6 strict concurrency, AVFoundation pipelines, Metal rendering, on-device speech.

For five months I worked in the Mobile Apps team at **Axis Communications** in Lund. I shipped Swift and SwiftUI features and bug fixes in an established production codebase — live-video controls for microphone, speaker and PTZ, an interactive SwiftUI Canvas interface, and a migration of selected asynchronous flows to `async/await` under strict Swift Concurrency requirements. I instrumented a multi-step workflow with Datadog and OpenTelemetry so failures could be traced instead of guessed at. Every task went through pull request, code review, testing and QA alongside iOS and Android developers.

Since then I have built my own projects end to end: architecture, tests, CI, documentation, release. I am looking for an iOS role in Skåne or across the bridge where code quality and knowledge sharing shape the daily work.

*iOS-utvecklare i Malmö/Lund. Öppen för roller i Skåne, Öresundsregionen och Köpenhamn.*

---

## Selected work

### [MetalVisualKit](https://github.com/antonsmedberg/MetalVisualKit) — GPU rendering as a Swift package

![License](https://img.shields.io/github/license/antonsmedberg/MetalVisualKit?style=flat-square)
![Last commit](https://img.shields.io/github/last-commit/antonsmedberg/MetalVisualKit?style=flat-square)

An MIT-licensed SPM package for GPU-first UI on iOS: a Metal compute simulation of roughly 1,400 particles, and a LiDAR point-cloud renderer that unprojects about 49,000 points per frame on the GPU.

`Swift` `Metal` `MetalKit` `ARKit` `SwiftUI` `Swift Package Manager` `DocC` `GitHub Actions`

<details>
<summary>Engineering details</summary>

- 15-test suite covering the compute pipeline, run in CI on every push
- Example app shipped in the repo, DocC archive built from source
- Custom `depthPalette()` instead of the standard turbo colormap
- Verified in an iOS 26.5 simulator with Xcode 26.6; on-device LiDAR validation is the remaining step before the v0.1.0 tag

</details>

### [DeviceMonitor](https://github.com/antonsmedberg/DeviceMonitor) — degree project, device status and history

An iOS app for viewing device state over time, built to be readable and testable rather than clever. Service, storage and view-model boundaries are separated, persistence is local, and the test suite runs in CI.

`Swift` `SwiftUI` `SwiftData` `MVVM` `Swift Concurrency` `XCTest` `XCUITest` `GitHub Actions`

<details>
<summary>Engineering details</summary>

- Six unit tests plus a UI smoke test, run on GitHub Actions
- Search and filtering over persisted history
- Written as my final project (examensarbete) and kept as a reference for how I structure a codebase

</details>

### Subtl — on-device video captioning *(in development)*

Captions for short-form video, generated entirely on device with Apple's SpeechAnalyzer and SpeechTranscriber. No uploads, no account. The transcription engine is an actor, the app is built under Swift 6 strict concurrency, and preview and export are held to the same rendering result so what you see is what you get out.

`Swift 6` `SpeechAnalyzer` `AVFoundation` `Core Animation` `os.Logger` `StoreKit 2`

<details>
<summary>Engineering details</summary>

- Five caption styles (Karaoke, Boxed, Clean, Pop, Typewriter) driven by a single style source of truth
- Export composed with `AVVideoCompositionCoreAnimationTool`; preview/export parity enforced
- Zero third-party dependencies — AVFoundation's hardware acceleration removed the case for FFmpeg
- Signpost instrumentation for stage timing; Metal effects stay out until profiling justifies them

</details>

---

## Experience

**iOS Developer, LIA — Mobile Apps** · Axis Communications, Lund · Jan–May 2026
Live-video controls (microphone, speaker, PTZ), SwiftUI Canvas interface, `async/await` migration under strict concurrency, Datadog/OpenTelemetry instrumentation. Jira-based agile workflow: refinement, pull requests, code review, QA.

**Android Developer, Internship** · Weavy, Malmö · Apr–Nov 2023
Android chat app in Kotlin and Jetpack Compose with authentication, API integrations and responsive UI.

## Education

**Java Developer — Backend & Web Development** · Grit Academy · 2024–2026
Higher Vocational Education (Yrkeshögskoleexamen, EQF/SeQF level 5): Java, Spring Boot, JPA, SQL, REST APIs, testing, Git-based workflows.

**iPhone & Android Application Development** · Malmö Yrkeshögskola · 2022–2023
Swift/iOS, Kotlin/Android, UX. Additional coursework in on-device ML, Python for AI, testing and digital accessibility.

## Stack

**iOS** — Swift · SwiftUI · UIKit · Swift Concurrency · async/await · actors · Combine · SwiftData · AVFoundation · Metal/MetalKit · ARKit · SpeechAnalyzer · MVVM · SPM · accessibility

**Quality & delivery** — Xcode · XCTest · XCUITest · Git · GitHub Actions · CI · code review · debugging · QA · Jira · Datadog · OpenTelemetry

**Also** — Kotlin · Jetpack Compose · Java · Spring Boot · REST APIs · SQL · JPA · GraphQL

## Languages

Swedish (native) · English (professional working proficiency) · reading Danish

---

<div align="center">

[Portfolio](https://antonsmedberg.github.io/) · [LinkedIn](https://www.linkedin.com/in/anton-smedberg-a9aa6121b/) · [anton@smedberg.eu](mailto:anton@smedberg.eu)

A written recommendation from an Engineering Manager at Axis Communications is available on request.

</div>
