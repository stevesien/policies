# policies

Privacy policies for my iOS apps, served as a static site by GitHub Pages.

| App | English | 日本語 |
| --- | --- | --- |
| WhenWasI | [whenwasi.html](https://stevesien.github.io/policies/whenwasi.html) | [whenwasi-ja.html](https://stevesien.github.io/policies/whenwasi-ja.html) |
| Yaoki · 八起き | [yaoki.html](https://stevesien.github.io/policies/yaoki.html) | [yaoki-ja.html](https://stevesien.github.io/policies/yaoki-ja.html) |

These URLs are what App Store Connect points at, under
**App Privacy → Privacy Policy URL**, per app and per localisation.

## Notes

- `wherewasi.html` is a redirect stub. The app was renamed WhereWasI → WhenWasI;
  the stub is only there so the old URL does not dead-end if it was handed out.
- `.nojekyll` stops Pages running the files through Jekyll, so the HTML is
  served exactly as written.
- These pages are the single source of truth. Do not keep a second copy inside
  an app repo — the two will drift, and the published one is the one that counts.

## Editing

Plain HTML, one shared `style.css`. Change the "Last updated" line whenever the
substance changes. If a change is material, note it in the App Store release
notes too, since neither app has a way to contact its users.

Both policies describe actual app behaviour and were written against the source.
If either app gains networking, an SDK, or a new permission, the policy has to
change in the same commit.
