Title: This Week in Rust 594
Number: 594
Date: 2025-04-09
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](https://www.rust-lang.org/) is a programming language empowering everyone to build reliable and efficient software.
This is a weekly summary of its progress and community.
Want something mentioned? Tag us at [@ThisWeekInRust](https://x.com/ThisWeekInRust) on X (formerly Twitter) or [@ThisWeekinRust](https://mastodon.social/@thisweekinrust) on mastodon.social, or [send us a pull request](https://github.com/rust-lang/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/rust-lang/this-week-in-rust) and archives can be viewed at [this-week-in-rust.org](https://this-week-in-rust.org/).
If you find any errors in this week's issue, [please submit a PR](https://github.com/rust-lang/this-week-in-rust/pulls).

Want TWIR in your inbox? [Subscribe here](https://this-week-in-rust.us11.list-manage.com/subscribe?u=fd84c1c757e02889a9b08d289&id=0ed8b72485).

## Updates from Rust Community

<!--

Dear community contributors:
Please read README.md for guidance on submissions.
Each submitted link should be of the form:

* [Title of the Linked Page](https://example.com/my_article)

If you don't know which category to use, feel free to submit a PR anyway
and just ask the editors to select the category.

-->

### Official

### Foundation

### Newsletters

### Project/Tooling Updates
* [zxc: A Terminal based mitm proxy written in rust with Tmux and Vim as user interface](https://hail-hydrant.github.io/zxc/)

### Observations/Thoughts
* [Replicating state changes across language barriers with Rust, UniFFI, and proc macros](https://www.tantaluspath.com/tech/rust_to_swift_state_syncing/)

* [Deterministic simulation testing for async Rust](https://s2.dev/blog/dst)

* [Things fall apart](https://bitfieldconsulting.com/posts/things-fall-apart)

### Rust Walkthroughs

### Research

### Miscellaneous

## Crate of the Week

<!-- COTW goes here -->

[Please submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

## Calls for Testing
An important step for RFC implementation is for people to experiment with the
implementation and give feedback, especially before stabilization.

If you are a feature implementer and would like your RFC to appear in this list, add a 
`call-for-testing` label to your RFC along with a comment providing testing instructions and/or 
guidance on which aspect(s) of the feature need testing.

* *No calls for testing were issued this week by [Rust](https://github.com/rust-lang/rust/labels/call-for-testing),
  [Rust language RFCs](https://github.com/rust-lang/rfcs/issues?q=label%3Acall-for-testing) or
  [Rustup](https://github.com/rust-lang/rustup/labels/call-for-testing).*

[Let us know](https://github.com/rust-lang/this-week-in-rust/issues) if you would like your feature to be tracked as a part of this list.

## Call for Participation; projects and speakers

### CFP - Projects

Always wanted to contribute to open-source projects but did not know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

<!-- CFPs go here, use this format: * [project name - title of issue](URL to issue) -->
<!-- * [ - ]() -->
<!-- or if none - *No Calls for participation were submitted this week.* -->

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines] or through a [PR to TWiR](https://github.com/rust-lang/this-week-in-rust) or by reaching out on [X (formerly Twitter)](https://x.com/ThisWeekInRust) or [Mastodon](https://mastodon.social/@thisweekinrust)!

[guidelines]:https://github.com/rust-lang/this-week-in-rust?tab=readme-ov-file#call-for-participation-guidelines

### CFP - Events

Are you a new or experienced speaker looking for a place to share something cool? This section highlights events that are being planned and are accepting submissions to join their event as a speaker.

<!-- CFPs go here, use this format: * [**event name**](URL to CFP)| Date CFP closes in YYYY-MM-DD | city,state,country | Date of event in YYYY-MM-DD -->
<!-- or if none - *No Calls for papers or presentations were submitted this week.* -->

If you are an event organizer hoping to expand the reach of your event, please submit a link to the website through a [PR to TWiR](https://github.com/rust-lang/this-week-in-rust) or by reaching out on [X (formerly Twitter)](https://x.com/ThisWeekInRust) or [Mastodon](https://mastodon.social/@thisweekinrust)!

## Updates from the Rust Project

<!-- Rust updates go here -->

### Rust Compiler Performance Triage

A busy week with lots of performance improvements. The largest performance improvement was from a revert of a previous week's regression just in time for the beta release. Another large improvement came to small tweaks in the query system showing that there still are opportunities for small, targeted performance improvements in the compiler.

Triage done by **@rylev**.
Revision range: [2ea33b59..e643f59f](https://perf.rust-lang.org/?start=2ea33b591050c4ca1a3752830b29112638faecf6&end=e643f59f6da3a84f43e75dea99afaa5b041ea6bf&absolute=false&stat=instructions%3Au)

**Summary**:

| (instructions:u)                   | mean  | range           | count |
|:----------------------------------:|:-----:|:---------------:|:-----:|
| Regressions ❌ <br /> (primary)    | 0.8%  | [0.2%, 1.9%]    | 11    |
| Regressions ❌ <br /> (secondary)  | 8.4%  | [0.2%, 38.5%]   | 16    |
| Improvements ✅ <br /> (primary)   | -1.0% | [-35.1%, -0.2%] | 206   |
| Improvements ✅ <br /> (secondary) | -1.8% | [-8.6%, -0.1%]  | 155   |
| All ❌✅ (primary)                 | -0.9% | [-35.1%, 1.9%]  | 217   |


2 Regressions, 9 Improvements, 5 Mixed; 4 of them in rollups
48 artifact comparisons made in total

[Full report here](https://github.com/rust-lang/rustc-perf/blob/28767e0a09d14829c2930a7e0c22ee73b0b0a4e7/triage/2025-04-08.md).

### [Approved RFCs](https://github.com/rust-lang/rfcs/commits/master)

Changes to Rust follow the Rust [RFC (request for comments) process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* *No RFCs were approved this week.*

### Final Comment Period

Every week, [the team](https://www.rust-lang.org/team.html) announces the 'final comment period' for RFCs and key PRs
which are reaching a decision. Express your opinions now.

#### Tracking Issues & PRs
##### [Rust](https://github.com/rust-lang/rust/issues?q=is%3Aopen+label%3Afinal-comment-period+sort%3Aupdated-desc)
* [f*::NAN: guarantee that this is a quiet NaN](https://github.com/rust-lang/rust/pull/139483)
* [Stabilize let chains in the 2024 edition](https://github.com/rust-lang/rust/pull/132833)
* [Stabilize the cell_update feature](https://github.com/rust-lang/rust/pull/134446)
* [Stabilize `-Zdwarf-version` as `-Cdwarf-version`](https://github.com/rust-lang/rust/pull/136926)
* [indirect-const-stabilize the `exact_div` intrinsic](https://github.com/rust-lang/rust/pull/139163)
* [Promise `array::from`_fn is generated in order of increasing indices](https://github.com/rust-lang/rust/pull/139099)

#### Other Areas
* *No Items entered Final Comment Period this week for
  [Rust RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period),
  [Cargo](https://github.com/rust-lang/cargo/issues?q=is%3Aopen+label%3Afinal-comment-period+sort%3Aupdated-desc),
  [Language Team](https://github.com/rust-lang/lang-team/issues?q=is%3Aopen+label%3Afinal-comment-period+sort%3Aupdated-desc+),
  [Language Reference](https://github.com/rust-lang/reference/issues?q=is%3Aopen+label%3Afinal-comment-period+sort%3Aupdated-desc) or
  [Unsafe Code Guidelines](https://github.com/rust-lang/unsafe-code-guidelines/issues?q=is%3Aopen+label%3Afinal-comment-period+sort%3Aupdated-desc).*

Let us know if you would like your PRs, Tracking Issues or RFCs to be tracked as a part of this list.

#### [New and Updated RFCs](https://github.com/rust-lang/rfcs/pulls)
* *No New or Updated RFCs were created this week.*

## Upcoming Events

Rusty Events between 2025-04-09 - 2025-05-07 🦀

### Virtual
* 2025-04-02 | Virtual (Indianapolis, IN, US) | [Indy Rust](https://www.meetup.com/indyrs/events/)
    * [**Indy.rs - with Social Distancing**](https://www.meetup.com/indyrs/events/302031661)
* 2025-04-03 | Virtual (Nürnberg, DE) | [Rust Nurnberg DE](https://www.meetup.com/rust-noris/)
    * [**Rust Nürnberg online**](https://www.meetup.com/rust-noris/events/300820282/)
* 2025-04-03 | Virtual | [Ardan Labs](https://www.eventbrite.com/o/ardan-labs-7092394651)
    * [**Communicate with Channels in Rust**](https://www.eventbrite.com/e/communicate-with-channels-in-rust-tickets-1278267335009)
* 2025-04-05 | Virtual (Kampala, UG) | [Rust Circle Meetup](https://www.eventbrite.com/o/rust-circle-kampala-65249289033)
    * [**Rust Circle Meetup**](https://www.eventbrite.com/e/rust-circle-meetup-tickets-628763176587)
* 2025-04-08 | Virtual (Dallas, TX, US) | [Dallas Rust User Meetup](https://www.meetup.com/dallasrust/events/)
    * [**Second Tuesday**](https://www.meetup.com/dallasrust/events/303522530)
* 2025-04-10 | Virtual (Berlin, DE) | [Rust Berlin](https://www.meetup.com/rust-berlin/events/)
    * [**Rust Hack and Learn**](https://www.meetup.com/rust-berlin/events/300820298)
* 2025-04-15 | Virtual (Washington, DC, US) | [Rust DC](https://www.meetup.com/rustdc/events/)
    * [**Mid-month Rustful**](https://www.meetup.com/rustdc/events/305170698)
* 2025-04-16 | Virtual (Vancouver, BC, CA) | [Vancouver Rust](https://www.meetup.com/vancouver-rust/events/)
    * [**Rust Study/Hack/Hang-out**](https://www.meetup.com/vancouver-rust/events/306231500)
* 2025-04-17 | Virtual and In-Person (Redmond, WA, US) | [Seattle Rust User Group](https://www.meetup.com/join-srug/events/)
    * [**April, 2025 SRUG (Seattle Rust User Group) Meetup**](https://www.meetup.com/seattle-rust-user-group/events/305658454)
* 2025-04-22 | Virtual (Dallas, TX, US) | [Dallas Rust User Meetup](https://www.meetup.com/dallasrust/events/)
    * [**Fourth Tuesday**](https://www.meetup.com/dallasrust/events/305361432)
* 2025-04-23 | Virtual (Cardiff, UK) | [Rust and C++ Cardiff](https://www.meetup.com/rust-and-c-plus-plus-in-cardiff/events/)
    * [**Beyond embedded - OS development in Rust **](https://www.meetup.com/rust-and-c-plus-plus-in-cardiff/events/307036053)
* 2025-04-24 | Virtual (Berlin, DE) | [Rust Berlin](https://www.meetup.com/rust-berlin/events/)
    * [**Rust Hack and Learn**](https://www.meetup.com/rust-berlin/events/300820299)
* 2025-04-24 | Virtual (Charlottesville, VA, US) | [Charlottesville Rust Meetup](https://www.meetup.com/charlottesville-rust-meetup/events/)
    * [**Part 2: Quantum Computers Can’t Rust-Proof This!"**](https://www.meetup.com/charlottesville-rust-meetup/events/306679733)

### Asia
* 2025-04-05 | Bangalore/Bengaluru, IN | [Rust Bangalore](https://hasgeek.com/rustbangalore)
    * [**April 2025 Rustacean meetup**](https://hasgeek.com/rustbangalore/april-2025-rustacean-meetup/)
* 2025-04-22 | Tel Aviv-Yafo, IL | [Rust 🦀 TLV](https://www.meetup.com/rust-tlv/events/)
    * [**In person Rust April 2025 at Braavos in Tel Aviv in collaboration with StarkWare**](https://www.meetup.com/rust-tlv/events/306530984)

### Europe
* 2025-04-02 | Cambridge, UK | [Cambridge Rust Meetup](https://www.meetup.com/cambridge-rust-meetup/events/)
    * [**Monthly Rust Meetup**](https://www.meetup.com/cambridge-rust-meetup/events/306553077)
* 2025-04-02 | Köln, DE | [Rust Cologne](https://www.meetup.com/rust-cologne-bonn/events/)
    * [**Rust in April: Rust Embedded, Show and Tell**](https://www.meetup.com/rustcologne/events/306940549)
* 2025-04-02 | München, DE | [Rust Munich](https://www.meetup.com/rust-munich/events/)
    * [**Rust Munich 2025 / 1 - hybrid**](https://www.meetup.com/rust-munich/events/306097261)
* 2025-04-02 | Oxford, UK | [Oxford Rust Meetup Group](https://www.meetup.com/oxford-rust-meetup-group/events/)
    * [**Oxford Rust and C++ social**](https://www.meetup.com/oxford-rust-meetup-group/events/306541535)
* 2025-04-02 | Stockholm, SE | [Stockholm Rust](https://www.meetup.com/stockholm-rust/events/)
    * [**Rust Meetup @Funnel**](https://www.meetup.com/stockholm-rust/events/306627608)
* 2025-04-03 | Oslo, NO | [Rust Oslo](https://www.meetup.com/rust-oslo/events/)
    * [**Rust Hack'n'Learn at Kampen Bistro**](https://www.meetup.com/rust-oslo/events/305809680)
* 2025-04-08 | Olomouc, CZ | [Rust Moravia](https://www.meetup.com/rust-moravia/events/)
    * [**3. Rust Moravia Meetup (Real Embedded Rust)**](https://www.meetup.com/rust-moravia/events/306377283)
* 2025-04-09 | Girona, ES | [Rust Girona](https://lu.ma/rust-girona)
    * [**Rust Girona Hack & Learn 04 2025**](https://lu.ma/dlvfol30)
* 2025-04-09 | Reading, UK | [Reading Rust Workshop](https://www.meetup.com/reading-rust-workshop/events/)
    * [**Reading Rust Meetup**](https://www.meetup.com/reading-rust-workshop/events/305045446)
* 2025-04-10 | Karlsruhe, DE | [Rust Hack & Learn Karlsruhe](https://www.meetup.com/rust-hack-learn-karlsruhe/events/)
    * [**Karlsruhe Rust Hack and Learn Meetup bei BlueYonder**](https://www.meetup.com/rust-hack-learn-karlsruhe/events/306682264)
* 2025-04-15 | Leipzig, DE | [Rust - Modern Systems Programming in Leipzig](https://www.meetup.com/rust-modern-systems-programming-in-leipzig/events/)
    * [**Topic TBD**](https://www.meetup.com/rust-modern-systems-programming-in-leipzig/events/305741632)
* 2025-04-15 | London, UK | [Women in Rust](https://www.meetup.com/women-in-rust/events/)
    * [**WIR x WCC: Finding your voice in Tech**](https://www.meetup.com/women-in-rust/events/306774769)
* 2025-04-19 | Istanbul, TR | [Türkiye Rust Community](https://kommunity.com/turkiye-rust-community/events)
    * [**Rust Konf Türkiye**](https://kommunity.com/turkiye-rust-community/events/rust-konf-turkiye-91f7b3a6)
* 2025-04-23 | London, UK | [London Rust Project Group](https://www.meetup.com/london-rust-project-group/events/)
    * [**Fusing Python with Rust using raw C bindings**](https://www.meetup.com/london-rust-project-group/events/306644439)
* 2025-04-24 | Aarhus, DK | [Rust Aarhus](https://www.meetup.com/rust-aarhus/events/)
    * [**Talk Night at MFT Energy**](https://www.meetup.com/rust-aarhus/events/305809344)
* 2025-04-24 | Edinburgh, UK | [Rust and Friends](https://www.meetup.com/rust-edi/events/)
    * [**Rust and Friends (evening pub)**](https://www.meetup.com/rust-and-friends/events/306911347)
* 2025-04-24 | Manchester, UK | [Rust Manchester](https://www.meetup.com/rust-manchester/events/)
    * [**Rust Manchester April Code Night**](https://www.meetup.com/rust-manchester/events/306899063)
* 2025-04-25 | Edinburgh, UK | [Rust and Friends](https://www.meetup.com/rust-edi/events/)
    * [**Rust and Friends (daytime coffee)**](https://www.meetup.com/rust-and-friends/events/306911357)
* 2025-04-29 | Paris, FR | [Rust Paris](https://www.meetup.com/rust-paris/events/)
    * [**Rust meetup #76**](https://www.meetup.com/rust-paris/events/306952202)

### North America
* 2025-04-03 | Chicago, IL, US | [Chicago Rust Meetup](https://www.meetup.com/chicago-rust-meetup/events/)
    * [**Rust Happy Hour**](https://www.meetup.com/chicago-rust-meetup/events/306728493)
* 2025-04-03 | Montréal, QC, CA | [Rust Montréal](https://www.meetup.com/rust-montreal/events/)
    * [**April Monthly Social**](https://www.meetup.com/rust-montreal/events/306518514/)
* 2025-04-03 | Saint Louis, MO, US | [STL Rust](https://www.meetup.com/stl-rust/events/)
    * [**icu4x - resource-constrained internationalization (i18n)**](https://www.meetup.com/stl-rust/events/304890140)
* 2025-04-06 | Boston, MA, US | [Boston Rust Meetup](https://www.meetup.com/bostonrust/events/)
    * [**Kendall Rust Lunch, Apr 6**](https://www.meetup.com/bostonrust/events/306844327)
* 2025-04-08 | New York, NY, US | [Rust NYC](https://www.meetup.com/rust-nyc/events/)
    * [**Rust NYC: Building a full-text search Postgres extension in Rust**](https://www.meetup.com/rust-nyc/events/306983122)
* 2025-04-10 | Portland, OR, US | [PDXRust](https://www.meetup.com/pdxrust/events/)
    * [**TetaNES: A Vaccination for Rust—No Needle, Just the Borrow Checker**](https://www.meetup.com/pdxrust/events/306714209)
* 2025-04-14 | Boston, MA, US | [Boston Rust Meetup](https://www.meetup.com/bostonrust/events/)
    * [**Coolidge Corner Brookline Rust Lunch, Apr 14**](https://www.meetup.com/bostonrust/events/306844334)
* 2025-04-17 | Nashville, TN, US | [Music City Rust Developers](https://www.meetup.com/music-city-rust-developers/events/)
    * [**Using Rust For Web Series 1 : Why HTMX Is Bad**](https://www.meetup.com/music-city-rust-developers/events/304333092)
* 2025-04-17 | Redmond, WA, US | [Seattle Rust User Group](https://www.meetup.com/join-srug/events/)
    * [**April, 2025 SRUG (Seattle Rust User Group) Meetup**](https://www.meetup.com/seattle-rust-user-group/events/305658454)
* 2025-04-23 | Austin, TX, US | [Rust ATX](https://www.meetup.com/rust-atx/events/)
    * [**Rust Lunch - Fareground**](https://www.meetup.com/rust-atx/events/xvkdgtyhcgbfc)
* 2025-04-25 | Boston, MA, US | [Boston Rust Meetup](https://www.meetup.com/bostonrust/events/)
    * [**Ball Square Rust Lunch, Apr 25**](https://www.meetup.com/bostonrust/events/306844343)

### Oceania
* 2025-04-09 | Sydney, NS, AU | [Rust Sydney](https://www.meetup.com/rust-sydney/events/)
    * [**Crab 🦀 X 🕳️🐇**](https://www.meetup.com/rust-sydney/events/306978026)
* 2025-04-14 | Christchurch, NZ | [Christchurch Rust Meetup Group](https://www.meetup.com/christchurch-rustlang-meetup-group/events/)
    * [**Christchurch Rust Meetup**](https://www.meetup.com/christchurch-rustlang-meetup-group/events/306841248)
* 2025-04-22 | Barton, AC, AU | [Canberra Rust User Group](https://www.meetup.com/rust-canberra/events/)
    * [**April Meetup**](https://www.meetup.com/rust-canberra/events/306425557)

### South America
* 2025-04-03 | Buenos Aires, AR | [Rust en Español](https://www.meetup.com/rust-argentina/events/)
    * [**Abril - Lambdas y más!**](https://www.meetup.com/rust-argentina/events/306671000)

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

## Jobs
<!--

Rust Jobs:

TWiR has stopped featuring individual job postings. You can read more about this change here:

https://github.com/rust-lang/this-week-in-rust/issues/3412

-->

Please see the latest [Who's Hiring thread on r/rust](INSERT_LINK_HERE)

# Quote of the Week

<!-- QOTW goes here -->

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq), [cdmistman](https://github.com/cdmistman), [ericseppanen](https://github.com/ericseppanen), [extrawurst](https://github.com/extrawurst), [U007D](https://github.com/U007D), [joelmarcey](https://github.com/joelmarcey), [mariannegoldin](https://github.com/mariannegoldin), [bennyvasquez](https://github.com/bennyvasquez), [bdillo](https://github.com/bdillo)*

*Email list hosting is sponsored by [The Rust Foundation](https://foundation.rust-lang.org/)*

<small>[Discuss on r/rust](REDDIT_LINK_HERE)</small>
