# Resources Downloader privacy policy

Last updated: August 30, 2026

Resources Downloader is designed to process page resources locally in your
browser. It does not collect product analytics and does not sell personal data.

## What the extension processes

When you start a scan, Resources Downloader can inspect the current page and
observe HTTP(S) resources loaded while that user-requested scan is active. It
uses this information to show previews, filters, file metadata, and download
choices. Multi-page collection opens only the URLs you paste, in inactive tabs,
and closes those tabs after scanning.

The extension temporarily stores current page titles, page URLs, resource URLs,
and scan results in `chrome.storage.session` so the side panel can survive a
service-worker restart. This session data is removed when the target tab closes
and is not sent to an analytics service.

The extension can store the following in `chrome.storage.local`:

- filter, naming, and saved site-setup preferences, including the site hostname
  and any search term you explicitly save;
- a one-time free-trial state;
- an encrypted Lemon Squeezy license key, activation instance ID, product
  variant ID, and last validation date when you activate Pro. The encryption
  key is non-extractable and kept separately by the browser in the extension's
  private IndexedDB storage.

The extension does not create a local or remote analytics profile. In
particular, it does not persist event totals, funnel milestones, active-day
history, page URLs, filenames, downloaded-file metadata, or file contents for
product measurement.

## Network services

Resources Downloader connects to:

- the pages and resource URLs you choose to scan or download;
- Lemon Squeezy when you open checkout or activate, validate, or deactivate a
  Pro license. Lemon Squeezy receives the checkout and license information
  needed to provide that service and applies its own privacy policy. Its
  License API can return purchase metadata such as the purchaser's name and
  email address in the response. The extension does not use or store those
  identity fields; they exist only transiently in the response held in memory;
- GitHub only when you choose a policy or support link.

The extension does not upload browsing history, scanned page contents, or
downloaded files to the publisher.

## Chrome Web Store Limited Use

Resources Downloader's use of information received from Chrome APIs complies
with the Chrome Web Store User Data Policy, including the Limited Use
requirements. Page and resource data is used only to provide and improve the
extension's disclosed bulk-resource workflow. It is not used for advertising,
credit decisions, or unrelated purposes; is not sold; and is not made available
for human review unless a user deliberately provides specific information for
support or disclosure is required for security or law.

## Permissions

The extension uses `scripting`, `webRequest`, `downloads`, `sidePanel`,
`storage`, and HTTP(S) host access for the user-visible scanning, multi-page,
ZIP, download, and local-state features described above. It does not use those
permissions to bypass authentication, paywalls, DRM, download limits, or other
access controls.

## Retention and control

Session scan data is temporary. Saved setups can be deleted in the extension.
You can remove all local data by clearing the extension's storage or
uninstalling it. Pro can be deactivated from the license dialog before clearing
local data so the activation becomes available for another browser.

A successful online license validation starts a 30-day offline grace period.
If a license is later disabled or refunded, Pro is removed at the next online
validation. A device that remains offline can retain cached access only until
that grace period expires.

## Support

Use the [support page](https://github.com/bouiboui/resources-downloader-support/issues/new)
for product issues or email [dev@cod3.net](mailto:dev@cod3.net), but never post
license keys, private page URLs, order details, or downloaded content in a
public issue. For order or refund matters, use email or reply to the private
contact information in your Lemon Squeezy receipt.

Material changes to this policy will be dated here and reflected in the Chrome
Web Store disclosure.
