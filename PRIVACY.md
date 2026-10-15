# Haul Browser Integration: Privacy Policy

Effective 15 October 2026

Haul Browser Integration ("the extension") connects your browser to Haul, a download manager that runs on your
own computer. This policy describes what the extension does with your data.

## What the extension reads

To hand a download to Haul, the extension reads the following on your device:

- **Download details:** the address of the file, the page it came from (address and title), the referrer, the
  file name, size and type.
- **Session details:**
  - the browser's cookies for the file's address
  - the browser's user agent and preferred language
  - for a download started by submitting a form, that form's data

  Haul needs these to download files that are only available while you are signed in.
- **Links:** the links on a page or in your selection, when you choose *Download all links with Haul* or
  *Download selected links with Haul*.
- **Media:** the addresses of video and audio streams a page loads, so the extension can list them in its
  toolbar popup and in the *Download video* button.
- **Clicks:** which mouse button and modifier keys were held when you clicked a link. Modifier keys are Alt or
  Option, plus the force key you set in Haul. The extension uses them to decide whether Haul should take the
  download. It does not record any other keystrokes or anything you type.

## Where the data goes

The extension sends this data only to the Haul app on the same computer, through the browser's native messaging.
The extension makes no network requests of its own. Haul uses the data only to download the files you asked for,
from the server that hosts them, as your browser would have done.

Neither the extension nor Haul sends your data to the developer or to anyone else. The data is not sold, not used
for advertising, profiling or creditworthiness, and not transferred to third parties.

## What the extension stores

The extension keeps these items in the browser's own extension storage on your device:

- the settings Haul gives it, such as the file types to capture, excluded sites and interface language
- the media detected in your open tabs (in session storage, which the browser clears when it closes)

Nothing is stored anywhere else.

## Limited Use

The use of information received from the extension adheres to the
[Chrome Web Store User Data Policy](https://developer.chrome.com/docs/webstore/program-policies/user-data-faq),
including the Limited Use requirements.

## Your choices

- Turn off **Capture downloads** in the extension's popup to stop handing downloads to Haul.
- Choose **Don't capture on this site** in the popup, or add the site to Haul's excluded sites, to leave a site
  alone.
- Removing the extension deletes everything it stored.

## Changes and contact

If this policy changes, the new version is published at this address with a new effective date. For questions,
use the contact email shown on the extension's Chrome Web Store listing.
