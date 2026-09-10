# policies

Support pages and privacy policies for my iOS apps, served as a static site by
GitHub Pages. (The repo name predates the support pages; it holds both.)

## URLs for App Store Connect

Both fields are per app *and* per localisation.

| App | | English | 日本語 |
| --- | --- | --- | --- |
| WhenWasI | Support | [whenwasi-support.html](https://stevesien.github.io/policies/whenwasi-support.html) | [whenwasi-support-ja.html](https://stevesien.github.io/policies/whenwasi-support-ja.html) |
| WhenWasI | Privacy | [whenwasi.html](https://stevesien.github.io/policies/whenwasi.html) | [whenwasi-ja.html](https://stevesien.github.io/policies/whenwasi-ja.html) |
| Yaoki · 八起き | Support | [yaoki-support.html](https://stevesien.github.io/policies/yaoki-support.html) | [yaoki-support-ja.html](https://stevesien.github.io/policies/yaoki-support-ja.html) |
| Yaoki · 八起き | Privacy | [yaoki.html](https://stevesien.github.io/policies/yaoki.html) | [yaoki-ja.html](https://stevesien.github.io/policies/yaoki-ja.html) |

A support URL is required for every app. A privacy policy URL is required for
both of these — Yaoki because it uses HealthKit, WhenWasI because it uses
background location.

## Notes

- `wherewasi.html` is a redirect stub. The app was renamed WhereWasI → WhenWasI;
  the stub is only there so the old URL does not dead-end if it was handed out.
- `.nojekyll` stops Pages running the files through Jekyll, so the HTML is
  served exactly as written.
- These pages are the single source of truth. Do not keep a second copy inside
  an app repo — the two will drift, and the published one is the one that counts.

## Editing

Plain HTML, one shared `style.css`. Change the "Last updated" line on a policy
whenever the substance changes. If a change is material, note it in the App
Store release notes too, since neither app has a way to contact its users.

Both policies describe actual app behaviour and were written against the source.
If either app gains networking, an SDK, or a new permission, the policy has to
change in the same commit. The support pages quote real UI labels, so they need
a look whenever those labels are reworded.
