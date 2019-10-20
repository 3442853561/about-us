# Rust UI Working Group [![Discord](https://img.shields.io/discord/634853209516802086?label=Discord)](https://discord.gg/RKWCECa)

This working group is open to anyone interested in participating. Please email kieseljake@gmail.com if you'd like to join us! Our 
objective is to build a UI system that focuses on using Rust as a first class language.

## Our goals

- Implementation language is Rust, unless interfacing with windowing or rendering technology that requires otherwise.
- Load and render declarative UI documents (File format undecided at this time).
- Support run-time modification of the UI state within Rust code.
- Thread safe API models.
- Support multiple rendering backends with graceful fallback.
- Where possible, use hardware accelerated rendering, i.e. render with the GPU.
- Support widely used computing platforms, such as Windows, OSX, Linux, Android, and iOS.


## Non-goals

- We are not interesting in rendering from HTML or CSS documents.
- We do not want to facilitate the design of one size fits all UI documents, for example, mobile and desktop
developers have diffent priorities and considerations, so each should make a UI document fit for their problem
space.
- We are not interested in supporting legacy hardware or software. This means technology that has been deprecated or replaced
by the original vendor. Exceptions can be made for legacy systems with significant userbases.
- While we welcome non-Rust language interfaces, we will never compromise the usability and quality of the Rust API
to meet their needs.

## F.A.Q.

- Are you endorsed by rust-lang?
  - Not yet!
- Is this an abstraction layer over native UI on each platform?
  - No. Each element in the UI model will come with a specification on how it should look when rendered. Additionally when
  designing the model no consideration will be given to the constraints imposed by native UI frameworks. That being said, if a
  third party were to implement a rendering backend using native UI widgets, and the final look and feel met the specification
  of the data model, who are we to stop them?
