# Homework problems

<aside>
<img src="https://www.notion.so/icons/briefcase_blue.svg" alt="https://www.notion.so/icons/briefcase_blue.svg" width="40px" /> **This is Part 10 of the Just Enough Prep Guide.** This workbook will explain why hiring managers request ‘homework problems’ and how you can use them to showcase your skillsets.

</aside>

“Homework” problems are increasingly popular as being closer to real work than single-function problems.

## The features of homework problems

Typically the features of such problems are:

- A standard time limit, usually not more than a few days.
- That time-limit clock starts at a time that you specify
    - so the clock begins fairly, in a timeframe when you can work around personal or day-job commitments.
- A project specification is handed to you at that time.
- Often within that spec are constraints on the technologies you can use.
- Sometimes you are given a starter skeleton codebase to work from.

## Some pitfalls to avoid

First let’s consider how many, many engineers end up crashing and burning on this problem genre.

- Encountering vague parts of the spec and just guessing what they mean without at least asking.
- When asking such questions, not framing them with enough context to make them easy for your company point-of-contact to answer.
- Writing code or tests very slowly because at your day job you are used to just copy-pasting starter chunks from elsewhere in your production codebase(s).
- Otherwise spending precious time looking up / recalling how to do basic things with your tools.
    - *Nothing’s wrong with looking things up, but at a certain point it will eat up too much of your time-limited time. Find the balance that works for you.*
- Writing code or tests very slowly because you are experimenting with:
    - a new language (if given your choice of language)
    - a new framework
    - a new IDE
    - a new keyboard layout (e.g., Dvorak)
    - *^^^ yes, maybe hard to believe, but we have seen all of these occur even in* ***live** interviews(!)*
- Otherwise spending precious time on environment setup.
- Similarly, spending precious time exploring which tools / libraries / frameworks you want to use.
- Not implementing, at minimum, exactly to the spec.
    - (It’s impressive — albeit usually unnecessary — to implement bonus features, but at least it needs to match the spec).
- Not dev-testing to check that the solution actually works.
- Not writing clean code.
- Not writing tests.
- Not writing enough tests.
- Not writing meaningful tests.
- Not writing a clear, professional-grade README.
    - Not a deal-killer, but given all the extra time to do homework, and its bias towards realism, you want to radiate professionalism and seeing things through.

## What to do to prepare

To prepare to deliver on homework projects efficiently and with sufficient quality, **make a project from scratch that is the opposite of the anti-patterns list above.**

If you need to warm up, follow a **paint-by-numbers tutorial project** first. **Then make the from-scratch project.**

Your project doesn’t have to be a super-original idea. It can be a tiny, partial clone of any existing app that you like, or it can be even another tutorial you find — but without following the tutorial per se.  

Make sure…

- you can do all the basic setup and housekeeping tasks prerequisite to the actual development.
- your IDE is fully set up for working on non-day-job projects, e.g., you have installed and are very familiar with using whatever plugins will help you.
- you have installed all frameworks and libraries you are likely to need.
- you can set up and write unit tests very fluently, almost from muscle memory.
- you can implement a single very-basic feature, including tests, in the above setup.
- you won’t get hung up on time-consuming tasks that are near-universal in your domain.

Let’s expand on that last point.

This can include:

- setting up simple auth
- setting up a container environment
- setting up and connecting to a database
    - if via an ORM, then be ready to work quickly your preferred ORM
    - if via raw SQL, then be ready to cleanly work with raw SQL in your code
- reading and writing common file formats (CSV, JSON)
- cleanly consuming a 3rd party network API
- setting up a ReST or GraphQL API
- setting up basic MVC
- setting up any common middleware
- if there is a UI, using a framework or a small bag of go-to techniques to quickly set up decent-looking layout and styling

The above list is just illustrative — it’s missing many possible items that emerge naturally from roles in data engineering, machine learning, devops, database design, and so forth.

## Your turn 👇

So come up with your own list that’s most appropriate for your own target roles.

The key is to spend a little time — over a weekend should suffice — getting all this stuff warmed up, de-rustified, and ready for you to work steadily and with minimal blockage.

You very likely already have done all this stuff on the job or in side projects. Just spend a little time marshaling the fundamental how-tos into your primary cache, and you’ll be fine.

<aside>
<img src="https://www.notion.so/icons/backward_blue.svg" alt="https://www.notion.so/icons/backward_blue.svg" width="40px" /> **Back: [System design problems](System%20design%20problems%201c511ab064a1836bb6b8817cf2a02d11.md)**

</aside>

<aside>
<img src="https://www.notion.so/icons/forward_blue.svg" alt="https://www.notion.so/icons/forward_blue.svg" width="40px" /> **Next: [Peer to Peer Feedback ](Peer%20to%20Peer%20Feedback%2073911ab064a1825ebaed813365d97ac6.md)**

</aside>

<aside>
<img src="https://www.notion.so/icons/home_blue.svg" alt="https://www.notion.so/icons/home_blue.svg" width="40px" /> Go Home: [The SWE’s Just Enough Prep Guide](../The%20SWE%E2%80%99s%20Just%20Enough%20Prep%20Guide%205e711ab064a183f99ffa01ace7bfa74d.md)

</aside>