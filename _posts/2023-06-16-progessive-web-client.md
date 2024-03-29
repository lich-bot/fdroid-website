---
layout: post
title: "Progressive web-app client for F-Droid"
author: "uniqx"
authorWebsite: "https://chaos.social/@uniqx"
---

We've created a prototype of a progressive [web app for browsing F-Droid
repositories](https://gitlab.com/uniqx/fdroid-webdash).  It's built with
[Flutter](https://flutter.dev/), which is really great for working in rapid
development cycles.  It also allows us to make it look and feel like a modern
Android app.  As a trade-off the web-app is pretty big in size (~ 10 MB).
So depending on your internet connection speed loading it for the first time
might take a while.  Flutter is also notorious for trying to connect to Google
servers, and we couldn't figure out how to make the app GDPR compliant just
yet.

Since it's a just an early prototype, it's nowhere near as complete as our
[official Android app](https://f-droid.org/packages/org.fdroid.fdroid/).
Right now it only has some of the most basic features: Displaying basic
repository informations; Providing a link/QR-code for adding the repository to
your F-Droid client; Browsing and searching for apps; Displaying app details
and app downloads.

F-Droid repositories themselves are deployed like web-sites.  So naturally it's
possible to deploy this web-app into any F-Droid repository and instantly make
it browse-able on the web.  We're considering adding an option for deploying it
automatically to our tools for managing F-Droid repositories.

The tooling that runs the F-Droid community can easily be applied to other
platforms like iOS. Our team came up with an
[experimental](https://gitlab.com/fdroid/fdroidserver/-/merge_requests/1275)
solution for shipping iOS apps using F-Droid repositories.  So our new PWA
opens up an opportunity to explore how F-Droid could offer a tiny taste of
freedom to iOS users.  While we hope to aid the expansion of free software
everywhere, even on proprietary platforms like iOS, F-Droid will only ship on
platforms that can be free software, like Android.
