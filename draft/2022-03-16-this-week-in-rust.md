Title: This Week in Rust 434
Number: 434
Date: 2022-03-16
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a programming language empowering everyone to build reliable and efficient software.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/rust-lang/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/rust-lang/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/rust-lang/this-week-in-rust/pulls).

## Updates from Rust Community

### Official

### Newsletters

### Project/Tooling Updates

* [Fornjot (Code-CAD in Rust) - Weekly Dev Log - 2022-W10](https://www.fornjot.app/blog/weekly-dev-log/2022-w10/)
- [Slint Version 0.2.1 released -- weekly update](https://slint-ui.com/thisweek/2022-03-14.html)

### Observations/Thoughts

### Rust Walkthroughs

* [Rust WebAssembly OCR experiments](https://hugopeixoto.net/articles/rust-wasm-ocr-experiments.html)

### Miscellaneous

* [audio] [Devtools podcast: building a new terminal in Rust](https://console.dev/podcast/s02e10-terminal-tools-michell-lim-zach-lloyd-warp/)

## Crate of the Week

This week's crate is [cfb](https://crates.io/crates/cfb), a crate to read/write Compound File Binary (structured storage) files.

Thanks to [Sebastian Urban](https://users.rust-lang.org/t/crate-of-the-week/2704/1034) for the suggestion!

[Please submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

## Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

## Updates from the Rust Project

343 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2022-02-28..2022-03-07

* [implement thread local cell methods](https://github.com/rust-lang/rust/pull/92123) (RFC [#3184](https://rust-lang.github.io/rfcs/3184-thread-local-cell-methods.html))
* [implement the `expect` attribute](https://github.com/rust-lang/rust/pull/87835) (RFC [#2383](https://rust-lang.github.io/rfcs/2383-lint-reasons.html))
* [`Adt` copy suggestions](https://github.com/rust-lang/rust/pull/94375)
* [do not point at whole file missing `fn main`](https://github.com/rust-lang/rust/pull/93142)
* [downgrade `#[test]` on macro call to warning](https://github.com/rust-lang/rust/pull/94624)
* [generalize "remove `&`"  and "add `*`" suggestions to more than one deref](https://github.com/rust-lang/rust/pull/91545)
* [lint against more useless `#[must_use]` attributes](https://github.com/rust-lang/rust/pull/93926)
* [improve `unexpected_cfgs` lint when their is no value expected](https://github.com/rust-lang/rust/pull/94561)
* [improve allowness of the `unexpected_cfgs` lint](https://github.com/rust-lang/rust/pull/94433)
* [improve error message for failed bitcode load](https://github.com/rust-lang/rust/pull/94672)
* [suggest adding a new lifetime parameter when two elided lifetimes should match up for traits and impls](https://github.com/rust-lang/rust/pull/94464)
* [suggest removing a semicolon after derive attributes](https://github.com/rust-lang/rust/pull/94633)
* [caching the stable hash of Ty within itself](https://github.com/rust-lang/rust/pull/94299)
* [clarify `Layout` interning](https://github.com/rust-lang/rust/pull/94690)
* [introduce `ConstAllocation`](https://github.com/rust-lang/rust/pull/94597)
* [chalk: recursive: fix hang on fulfill by slightly smarter check for progress](https://github.com/rust-lang/chalk/pull/752)
* [miri: make sure we notice when a u16 is loaded at offset 1 into a u8 allocation](https://github.com/rust-lang/miri/pull/1994)
* [miri: add more simd_reduce intrinsics](https://github.com/rust-lang/miri/pull/2001)
* [miri: adjust for div/rem overflow being UB](https://github.com/rust-lang/miri/pull/1992)
* [miri: also test f32/f64 simd_reduce](https://github.com/rust-lang/miri/pull/2003)
* [miri: implement missing SIMD comparison operators, simd_xor, and simd_reduce_all](https://github.com/rust-lang/miri/pull/2000)
* [miri: implement more SIMD intrinsics](https://github.com/rust-lang/miri/pull/2004)
* [miri: implement simd_neg and simd_fabs](https://github.com/rust-lang/miri/pull/1997)
* [miri: implement simd_saturating intrinsics](https://github.com/rust-lang/miri/pull/2007)
* [stabilize `const_fn_fn_ptr_basics`, `const_fn_trait_bound`, and `const_impl_trait`](https://github.com/rust-lang/rust/pull/93827)
* [add `#[track_caller]` to track callers when initializing poisoned `Once`](https://github.com/rust-lang/rust/pull/94236)
* [add `Atomic*::from_mut_slice`](https://github.com/rust-lang/rust/pull/94384)
* [portable SIMD: add bitmask i{N <8} -> u8 impls](https://github.com/rust-lang/portable-simd/pull/250)
* [futures: `Shared`: fix false detection of inner panics](https://github.com/rust-lang/futures-rs/pull/2576)
* [support GATs in Rustdoc](https://github.com/rust-lang/rust/pull/94009)
* [rustfmt: fix missing struct field separators under certain conditions](https://github.com/rust-lang/rustfmt/pull/5159)
* [rustfmt: prevent wrapping markdown headers in doc comments](https://github.com/rust-lang/rustfmt/pull/5242)
* [rustfmt: fallback to dir_path when relative external mod resolution fails](https://github.com/rust-lang/rustfmt/pull/5205)
* [clippy: add `unnecessary-find-map` lint](https://github.com/rust-lang/rust-clippy/pull/8489)
* [clippy: add lint to detect `allow` attributes without reason](https://github.com/rust-lang/rust-clippy/pull/8504)
* [clippy: lint for casting between raw slice pointers with different element sizes](https://github.com/rust-lang/rust-clippy/pull/8445)
* [clippy: new lint: `missing-spin-loop`](https://github.com/rust-lang/rust-clippy/pull/8174)
* [clippy: use `.into_iter()` rather than `.drain(..)`](https://github.com/rust-lang/rust-clippy/pull/8483)
* [clippy: check `use_self` in `pat`](https://github.com/rust-lang/rust-clippy/pull/8456)
* [clippy: omit `dbg-macro` in test code](https://github.com/rust-lang/rust-clippy/pull/8500)
* [clippy: optimize `redundant-clone`](https://github.com/rust-lang/rust-clippy/pull/8414)
* [clippy: `transmute-undefined-repr` to nursery again](https://github.com/rust-lang/rust-clippy/pull/8432)

### Rust Compiler Performance Triage

Largely a quiet week. The perf improvement highlight is the use of real world crates such as `syn`, `cargo`, and `serde` in the collecting of profile guided optimization (PGO) profiles. Previously only `libcore` was used. This led to some decent improvement in compilation of real world crates (upwards of 5.5%). 

On the regression side, the regressions were all largely small but contained inside of rollups making them hard to diagnose and correct. The perf team continues to work on process improvements that make changes to the compiler land through CI quickly while minimizing perf regressions that can sneak through.

Triage done by **@rylev**.
Revision range: [10dccdc..3ba1eb](https://perf.rust-lang.org/?start=10dccdc7fcbdc64ee9efe2c1ed975ab8c1d61287&end=3ba1ebea122238d1a5c613deb1bf60ce24bd8fd8&absolute=false&stat=instructions%3Au)

2 Regressions, 3 Improvements, 3 Mixed; 3 of them in rollups
42 comparisons made in total

[Full report here](https://github.com/rust-lang/rustc-perf/blob/master/triage/2022-03-15.md)

### [Approved RFCs](https://github.com/rust-lang/rfcs/commits/master)

Changes to Rust follow the Rust [RFC (request for comments) process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* [Cargo alternative registry auth](https://github.com/rust-lang/rfcs/pull/3139)

### Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

#### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

* *No RFCs entered Final Comment Period this week.*

#### [Tracking Issues & PRs](https://github.com/rust-lang/rust/issues?q=is%3Aopen+label%3Afinal-comment-period+sort%3Aupdated-desc)

* [disposition: merge] [Tracking Issue for JoinHandle::is_finished](https://github.com/rust-lang/rust/issues/90470)
* [disposition: merge] [Tracking issue for const extern fn and const unsafe extern fn](https://github.com/rust-lang/rust/issues/64926)
* [disposition: merge] [Always evaluate all cfg predicate in all() and any()](https://github.com/rust-lang/rust/pull/94295)

### [New and Updated RFCs](https://github.com/rust-lang/rfcs/pulls)

* [new] [RFC: Packages as (optional) namespaces](https://github.com/rust-lang/rfcs/pull/3243)

## Upcoming Events

Rusty Events between 2022-03-16 - 2022-04-13 🦀

### Virtual

* 2022-03-16 | Egg Harbor City, NJ, US | [Neighborhood Math Club](https://www.meetup.com/neighborhood-math-club/)
    * [**The Early Rustacean Gets The Worm!**](https://www.meetup.com/neighborhood-math-club/events/284221983/)
* 2022-03-16 | Seattle, WA, US | [Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/)
    * [**Monthly meetup**](https://www.meetup.com/Seattle-Rust-Meetup/events/gskksrydcfblb/)
* 2022-03-16 | Vancouver, BC, CA | [Vancouver Rust](https://www.meetup.com/Vancouver-Rust/)
    * [**Building a Randomizer**](https://www.meetup.com/Vancouver-Rust/events/nwcmpsydcfbvb/)
* 2022-03-17 | Stuttgart, DE | [Rust Community Stuttgart](https://www.meetup.com/Rust-Community-Stuttgart/)
    * [**Rust-Meetup**](https://www.meetup.com/Rust-Community-Stuttgart/events/lwgrssydcfbwb/)
* 2022-03-23 | Egg Harbor City, NJ, US | [Neighborhood Math Club](https://www.meetup.com/neighborhood-math-club/)
    * [**The Early Rustacean Gets The Worm!**](https://www.meetup.com/neighborhood-math-club/events/284379020/)
* 2022-03-24 | Charlottesville, VA, US | [Charlottesville Rust Meetup](https://www.meetup.com/Charlottesville-Rust-Meetup/)
    * [**Embedded Rust reaching out--Learn how Rust can interact with the outside world**](https://www.meetup.com/Charlottesville-Rust-Meetup/events/284627448/)
* 2022-03-24 | Linz, AU | [Rust Linz](https://www.meetup.com/Rust-Linz/)
    * [**Rust Meetup Linz - 20th Edition**](https://www.meetup.com/Rust-Linz/events/284584338/)
* 2022-03-29 | Berlin, DE | [Berline](https://berline.rs/)
    * [**Rust Hack and Learn Tuesday**](https://berline.rs/2022/03/29/rust-hack-and-learn.html)
* 2022-03-29 | Dallas, TX, US | [Dallas Rust](https://www.meetup.com/Dallas-Rust/)
    * [**Last Tuesday**](https://www.meetup.com/Dallas-Rust/events/jqxqwrydcfbmc/)
* 2022-03-30 | México City, MX | [Rust MX](https://www.meetup.com/Rust-MX/)
    * [**Platica Marzo 2022 - Reescribir o no reescribir aplicaciones en Rust**](https://www.meetup.com/Rust-MX/events/284560362/)
* 2022-04-05 | Beijing, CN | [WebAssembly and Rust Meetup (Rustlang)](https://www.meetup.com/Wasm-Rust-Meetup/)
    * [**Monthly WasmEdge Community Meeting, a CNCF sandbox WebAssembly runtime**](https://www.meetup.com/Wasm-Rust-Meetup/events/jbfnrsydcgbhb/)
* 2022-04-05 | Buffalo, NY, US | [Buffalo Rust Meetup](https://www.meetup.com/Buffalo-Rust-Meetup/)
    * [**Buffalo Rust User Group, First Tuesdays**](https://www.meetup.com/Buffalo-Rust-Meetup/events/xgmfssydcgbhb/)
* 2022-04-05 | Denver, CO, US | [Rust Denver](https://www.meetup.com/Rust-Boulder-Denver/)
    * [**Using Futures to wrap an unsafe USB API to play audio directly - with live stream**](https://www.meetup.com/Rust-Boulder-Denver/events/284371995/)
* 2022-04-06 | Egg Harbor City, NJ, US | [Neighborhood Math Club](https://www.meetup.com/neighborhood-math-club/)
    * [**The Early Rustacean Gets The Worm!**](https://www.meetup.com/neighborhood-math-club/events/kpgpssydcgbjb/)
* 2022-04-06 | Indianapolis, IN, US | [Indy Rust](https://www.meetup.com/indyrs/)
    * [**Indy.rs - with Social Distancing**](https://www.meetup.com/indyrs/events/qwtdjsydcgbjb/)
* 2022-04-07 | Nürnberg, DE | [Rust Nuremberg](https://www.meetup.com/rust-noris/)
    * [**Rust Nürnberg online #12**](https://www.meetup.com/rust-noris/events/zgfnssydcgbsb/)
* 2022-04-12 | Dallas, TX, US | [Dallas Rust](https://www.meetup.com/Dallas-Rust/)
    * [**Second Tuesday**](https://www.meetup.com/Dallas-Rust/events/vqtjcsydcgbqb/)
* 2022-04-12 | Seattle, WA, US | [Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/)
    * [**Monthly Meetup**](https://www.meetup.com/Seattle-Rust-Meetup/events/gskksrydcgbqb/)
* 2022-04-13 | Boulder, CO | [Boulder Elixir and Rust](https://www.meetup.com/boulder-elixir-rust/)
    * [**Monthly Meetup**](https://www.meetup.com/boulder-elixir-rust/events/zvxcsrydcgbrb/)
* 2022-04-13 | Egg Harbor City, NJ, US | [Neighborhood Math Club](https://www.meetup.com/neighborhood-math-club/)
    * [**The Early Rustacean Gets The Worm!**](https://www.meetup.com/neighborhood-math-club/events/kpgpssydcgbrb/)
* 2022-04-13 | Munich, DE | [Rust Munich](https://www.meetup.com/rust-munich/)
    * [**Rust Munich 2022 / 1 - hybrid**](https://www.meetup.com/rust-munich/events/283790509/)

### Europe
* 2022-03-17 | Edinburgh, UK | [Rust Edinburgh](https://www.meetup.com/rust-edi/)
    * [**Rust Night March, Edinburgh**](https://www.meetup.com/rust-edi/events/284428178/)
* 2022-04-12 | Berlin, DE | [Rust Berlin](https://www.meetup.com/Rust-Berlin/)
    * [**Rust and Tell - an onsite event**](https://www.meetup.com/Rust-Berlin/events/284512764/) | [**Alt Link**](https://berline.rs/2022/04/12/rust-and-tell.html)
* 2022-04-13 | Munich, DE | [Rust Munich](https://www.meetup.com/rust-munich/)
    * [**Rust Munich 2022 / 1 - hybrid**](https://www.meetup.com/rust-munich/events/283790509/)

### North America
* 2022-04-05 | Denver, CO, US | [Rust Denver](https://www.meetup.com/Rust-Boulder-Denver/)
    * [**Using Futures to wrap an unsafe USB API to play audio directly - with live stream**](https://www.meetup.com/Rust-Boulder-Denver/events/284371995/)
* 2022-04-13 | Atlanta, GA, US | [Rust ATL](https://www.meetup.com/Rust-ATL/)
    * [**Grab a beer with fellow Rustaceans**](https://www.meetup.com/Rust-ATL/events/pczdssydcgbrb/)

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

**Kollider**

* [Senior Frontend Engineer - Rust (Remote)](https://careers.kollider.xyz/senior-frontend-engineer/en)
* [Junior Backend Engineer - Rust (Remote)](https://careers.kollider.xyz/junior-backend-engineer/en)

**Tempus Ex**

 * [Several full-time Rust positions available (San Francisco, CA, US, Atlanta, GA, US, Austin, TX, US, and Remote)](https://tempus-ex.com/careers)

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> Because it is designed not to own. If you need an owning pointer, use Box.
>
> This is like asking "why there is no chocolate mousse in this burger?". Chocolate mousse is delicious, but it does not belong in a burger. If you want chocolate mousse, then that's fine and you can choose to eat it instead of a burger. But at other times you may want a burger instead.

– [H2CO3 answering why raw pointers don't own on rust-users](https://users.rust-lang.org/t/why-raw-pointer-doesnt-own-type-parameter-t-for-dropcheck/72408)

Thanks to [Deep Majumder](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1186) for the suggestion!

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq), [cdmistman](https://github.com/cdmistman), [ericseppanen](https://github.com/ericseppanen), [extrawurst](https://github.com/extrawurst), [andrewpollack](https://github.com/andrewpollack), [U007D](https://github.com/U007D), [kolharsam](https://github.com/kolharsam), [joelmarcey](https://github.com/joelmarcey), [mariannegoldin](https://github.com/mariannegoldin).*

*Email list hosting is sponsored by [The Rust Foundation](https://foundation.rust-lang.org/)*

<small>[Discuss on r/rust](https://www.reddit.com/r/rust/comments/k5nsab/this_week_in_rust_367/)</small>