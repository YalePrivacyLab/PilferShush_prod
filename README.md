# PilferShush: Detect near-ultrasonic &amp; ultrasonic signals

PilferShush listens for ultra-high frequencies, like the ones utilized by ultrasonic trackers such as [SilverPush](https://reports.exodus-privacy.eu.org/trackers/80/), [Alphonso](https://reports.exodus-privacy.eu.org/trackers/82/), [Lisnr](https://reports.exodus-privacy.eu.org/trackers/79/), [Shopkick](https://reports.exodus-privacy.eu.org/trackers/81/), [Signal360](https://reports.exodus-privacy.eu.org/trackers/86/), and [Fidzup](https://reports.exodus-privacy.eu.org/trackers/2/).  These signals are transmitted for purposes such as location tracking and consumer advertising, as [demonstrated in this video](https://www.youtube.com/watch?v=Xweq1eF_eP4).  Ultrasonic frequencies can be emitted from devices as small and covert as Internet-of-Things lightbulbs, as [demonstrated here](https://vimeo.com/183291077).  More often, however, signals are broadcast over retail speakers and [bluetooth beacons](https://hackaday.com/2017/05/04/ultrasonic-tracking-beacons/).

If an app on your phone has recording permissions, it may be using the microphone to detect these tones (inaudible to the human ear) and discover information about who you are, where you are, who and what you're near, and what you're doing at any specific moment.  Though SilverPush garnered international attention and [warnings from the U.S. Federal Trade Commission](https://www.ftc.gov/news-events/press-releases/2016/03/ftc-issues-warning-letters-app-developers-using-silverpush-code) in 2016, apps that utilize ultrasonic tracking are still prevalant.  In December 2017, a _New York Times_ article revealed that [Alphonso was tracking children](https://www.nytimes.com/2017/12/28/business/media/alphonso-app-tracking.html) through the interaction of televisions with kid's games.

PilferShush app also includes background scanners for intermittent polling of microphone use (triggers exceptions via AUDIO_FOCUS, etc), scanning user apps for known package names used by audio beacon SDKs as well as RECORD_AUDIO, BOOT, receivers and services.

# Release Notes

## Version 2.0
* Updated Android Studio build/release
  * minimum API 18 (4.3)
  * target API 23 (6.x)
  * compiled API 26 (8.x) 

testing devices  
* LOW : s4 I9195 (deprecated) 4.3.1 (18)(CyanogenMod 10.2, F-Droid)
* DEV : s5 G900I (tainted) 7.1.2 (25)(LineageOS 14.1, GApps)
* HIGH : s5 G900P (user) 7.1.2 (25)(LineageOS 14.1, F-Droid)

## TODO
* USB Audio routing test
* build for API 26, 8.x, 'O' and up features

# Design
[The Critical Engineering Manifesto](https://criticalengineering.org/) provides the methodological framework for all technological interactions.

# Who We Are
[Yale Privacy Lab](https://privacylab.yale.edu) explores the connection between privacy, security, and anonymity through hands-on software and hardware implementation. Yale Privacy Lab is an initiative of the [Information Society Project](https://www.law.yale.edu/isp) at Yale Law School.

# Author
[Kaputnik Go](https://github.com/kaputnikGo) received 1st Class Honours from RMIT University (Melbourne, Australia) with a research thesis titled: "Knowing and Not Knowing: The Problem of Privacy in an Internet-of-Things World."

# License
Copyright Kaputnik Go, released under the [GNU General Public License version 3 or later](https://www.gnu.org/licenses/gpl-3.0.en.html).

Screenshots (as of 2.0.26)

- App open
<img src="https://github.com/YalePrivacyLab/PilferShush_prod/blob/master/images/app-open.jpg" height="612px" />

- Detailed View
<img src="https://github.com/YalePrivacyLab/PilferShush_prod/blob/master/images/detailed-view.jpg" height="612px" />

- Capture live
<img src="https://github.com/YalePrivacyLab/PilferShush_prod/blob/master/images/capture-live.jpg" height="612px" />

- Post capture
<img src="https://github.com/YalePrivacyLab/PilferShush_prod/blob/master/images/post_capture.jpg" height="612px" />

- Option menu
<img src="https://github.com/YalePrivacyLab/PilferShush_prod/blob/master/images/option-menu.jpg" height="612px" />
