# EVWorks privacy policies

Public hosting for the privacy policies of EVWorks Android apps, served by
GitHub Pages. Public on purpose — Google Play, AdMob consent messages, and the
Google payments/merchant profile all require a publicly reachable URL.

## Layout

One directory per app, each with an `index.html`, so URLs stay directory-style
and survive a later move to a custom domain:

```
/                  → landing page listing the apps
/proteus/          → Proteus (com.evworks.proteus)
```

## Adding an app

Create `<app>/index.html` and add a row to the list in `/index.html`.

## Canonical source

**Do not edit `proteus/index.html` here as the source of truth.** It is a copy
of `docs/privacy.html` in the (private) Proteus repo, which is where the policy
is reviewed alongside the code that determines what it must disclose. Change it
there, then copy it here. Keeping the source next to the code is what stops the
policy drifting away from the app's actual data flows.

## Where these URLs are referenced

A URL here is quoted in three places per app — changing one means updating all
three:

1. Google payments/merchant profile
2. Play Console → Store presence → Privacy policy
3. AdMob → Privacy & messaging → the consent message
