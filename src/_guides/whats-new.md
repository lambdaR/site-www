---
title: What’s new
description: A list of what’s new on dart.dev and related sites.
---

This page describes what's new on the Dart website and blog.
To see what's new in Flutter, visit the
[Flutter what's new page.][flutter-whats-new]

For a list of Dart language changes in each Dart SDK, see the 
[language evolution page](/guides/language/evolution).
To stay on top of announcements, including breaking changes,
join the [Dart announcements Google group][dart-announce]
and follow the [Dart blog][].

[flutter-whats-new]: {{site.flutter}}/docs/whats-new
[dart-announce]: https://groups.google.com/a/dartlang.org/d/forum/announce
[Dart blog]: https://medium.com/dartlang


## March 3, 2021: 2.12 release

This section lists notable changes made from October 2, 2020,
through March 3, 2021.
For details about the 2.12 release, see [Announcing Dart 2.12][].


### Docs updated or added to dart.dev
{: .no_toc}

In addition to bug fixes and incremental improvements, we made the following changes to this site:

* Updated and fleshed out null safety docs. Notably:
  * Provided a [migration guide][].
  * Added a [FAQ][ns-faq].
  * Created [Unsound null safety][].
  * Simplified the [null safety homepage][].
* Refreshed [Effective Dart][], updating code to be null safe and
  changing rules to reflect new guidance.
* Refreshed the [language tour][], updating code to be null safe and
  adding information about new features such as
  [`late` variables][].
* Updated the [evolution page][] to add information about language versioning
  and to reflect Dart 2.12.
* Updated the [library tour][], [samples][], and [codelabs][]
  to reflect sound null safety.
* Updated pages across the site to use [the `dart` tool][]
  instead of deprecated commands.
  Started adding pages for various `dart` commands, including
  [`dart analyze`][], [`dart compile`][], [`dart fix`][],
  and [`dart format`][].
* Created a page documenting the quality and support of [Dart team packages][].
* Replaced the Platforms page with a new [Overview page][].
* Created this page ("What’s new").

We also switched from Travis CI to GitHub Actions, and we made multiple CSS changes to improve site legibility.

[Announcing Dart 2.12]: https://medium.com/dartlang/announcing-dart-2-12-499a6e689c87
[migration guide]: /null-safety/migration-guide
[ns-faq]: /null-safety/faq
[Unsound null safety]: /null-safety/unsound-null-safety
[null safety homepage]: /null-safety
[Overview page]: /overview
[Effective Dart]: /guides/language/effective-dart
[language tour]: /guides/language/language-tour
[`late` variables]: /guides/language/language-tour#late-variables
[library tour]: /guides/libraries/library-tour
[samples]: /samples
[codelabs]: /codelabs
[evolution page]: /guides/language/evolution
[the `dart` tool]: /tools/dart-tool
[`dart analyze`]: /tools/dart-analyze
[`dart compile`]: /tools/dart-compile
[`dart fix`]: /tools/dart-fix
[`dart format`]: /tools/dart-format
[Dart team packages]: /dart-team-packages


### Articles added to the Dart blog
{: .no_toc}

We published the following articles on the Dart blog:

* [Preparing the Dart and Flutter ecosystem for null safety][blog-2-16-21]
  announced null safety API stability and
  invited developers to publish stable, null-safe versions of their packages.
* [Dart and the performance benefits of sound types][blog-1-19-21]
  demonstrated how soundness and null safety enable Dart compilers to
  generate faster, smaller code.
* [Why nullable types?][blog-12-7-20]
  expanded on a discussion on the /r/dart_lang subreddit,
  answering the question “Why not get rid of null completely?”
* [Announcing Dart null safety beta][blog-11-19-20]
  invited developers to start planning their migration to null safety.

[blog-2-16-21]: https://medium.com/dartlang/preparing-the-dart-and-flutter-ecosystem-for-null-safety-e550ce72c010
[blog-1-19-21]: https://medium.com/dartlang/dart-and-the-performance-benefits-of-sound-types-6ceedd5b6cdc
[blog-12-7-20]: https://medium.com/dartlang/why-nullable-types-7dd93c28c87a
[blog-11-19-20]: https://medium.com/dartlang/announcing-dart-null-safety-beta-87610fee6730

## October 1, 2020: 2.10 release

This section lists notable changes made from
July 1 through October 1, 2020.
For details about the 2.10 release, see [Announcing Dart 2.10.][210-ann]

[210-ann]: https://medium.com/dartlang/announcing-dart-2-10-350823952bd5

<div class="no_toc_section" markdown="1">

### Docs updated or added to dart.dev
{: .no_toc}

In addition to bug fixes and small improvements,
we made the following changes to this site:

* Added a [`dart` tool page][dart-tool]
  to document the new command-line interface to the Dart SDK.
  The new `dart` tool is analogous to the `flutter` tool in the Flutter SDK.
  Previously, the `dart` command only ran command-line apps.
  We updated [the previous `dart` page][dart-vm] accordingly
  and plan to update references to other tools over time.
* Updated the [package changelog documentation][changelog-docs]
  to recommend a standard format for `CHANGELOG.md` files.
  This new format lets tools
  (such as the relaunched pub.dev)
  parse changelogs.
* Changed an [Effective Dart][] guideline to favor
  using `Object` instead of `dynamic`.
  For details, see the revised guideline
  [AVOID using `dynamic` unless you want to disable static checking.][dynamic]
* Updated the [diagnostic messages page][diagnostics] to
  include more messages produced by the Dart analyzer.
* Updated the [language evolution page][evolution]
  to include 2.9 and 2.10.
* Reorganized the [language specification page][spec]
  to make it easier to find the PDF version of
  the latest, in-progress specification.
* Added or updated docs related to [sound null safety][],
  a feature that's coming to the Dart language:
  * Clarified how to use [experiment flags with IDEs][experiments].
  * Updated the null safety page, adding information about
    [how to enable null safety][ns-enable].
  * Added a deep dive into null safety,
    [Understanding null safety][],
    written by Dart engineer Bob Nystrom.

[dart-tool]: /tools/dart-tool
[dart-vm]: /tools/dart-vm
[diagnostics]: /tools/diagnostic-messages
[dynamic]: /guides/language/effective-dart/design#avoid-using-dynamic-unless-you-want-to-disable-static-checking
[Effective Dart]: /guides/language/effective-dart
[evolution]: /guides/language/evolution
[experiments]: /tools/experiment-flags#using-experiment-flags-with-ides
[ns-enable]: /null-safety#enable-null-safety
[Understanding null safety]: /null-safety/understanding-null-safety
[sound null safety]: /null-safety
[diagnostics]: /tools/diagnostic-messages
[changelog-docs]: /tools/pub/package-layout#changelogmd
[spec]: /guides/language/spec

### Articles added to the Dart blog
{: .no_toc}

We published the following articles on the [Dart blog:][Dart blog]

* [Exploring collections in Dart][] helps you use collections
  (lists, maps, sets, and more), with specal attention to
  2.3 language features like collection if, collection for, and spreads.
* [Google Summer of Code 2020 results][] describes the results of
  five projects that the Dart team mentored.
* [Introducing a brand new pub.dev][] announces the relaunch of
  the [pub.dev site,][pub.dev] with new package scoring metrics, improved search,
  and a redesigned UI.

We also improved the blog navigation,
adding **announcement** and **archive** tabs, plus a link to dart.dev.

{{site.alert.tip}}
  All articles in the Dart blog are free to read.
{{site.alert.end}}

</div>

[Dart blog]: https://medium.com/dartlang
[Exploring collections in Dart]: https://medium.com/dartlang/exploring-collections-in-dart-f66b6a02d0b1
[Google Summer of Code 2020 results]: https://medium.com/dartlang/google-summer-of-code-2020-results-a38cd072c9fe
[Introducing a brand new pub.dev]: https://medium.com/dartlang/pub-dev-redesign-747406dcb486
[pub.dev]: {{site.pub}}
