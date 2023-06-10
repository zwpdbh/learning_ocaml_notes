# How to build fullstack web application in OCaml 

## General guide line 

It mainly depends on how to build frontend in OCaml. \
Currently the most promising solution is using React.

There are some context about React and OCaml:

- BuckleScript (replaced by ReScript)
- Reason
- ReasonML 
- ReasonReact (for writing React using Reason)
- ReScript


Summary 

- BuckleScript was a compiler with a standard library and some bindings for OCaml (with support for Reason syntax) rather than being its own language.
- Reason is merely a syntactical change of OCaml. i.e. ReasonML semantic has a bijection to OCaml semantic.
- ReasonML is the name given to the Reason ecosystem. More broadly construed, ReasonML is a community focused on popularizing OCaml with an emphasis on outreach to JS developers.
- BuckleScript is now replaced by ReScript.
- ReScript is combined of 
  - A JS-like syntax for OCaml (like Reason)
  - A compiler and toolchain (like BuckleScript)
  - A community and various tooling (like ReasonML)
- The biggest problem is: ReasonReact has BuckleScript helpers for creating components and using JSX but they only run if your code is written in ReasonML (not OCaml).
  
## How to get React-JSX to work with OCaml 




## References

- [OCaml and the Web](https://medium.com/@shawn.mcginty/ocaml-and-the-web-9c3a16fe90e6)
- [Server-side rendering React in OCaml](https://sancho.dev/blog/server-side-rendering-react-in-ocaml)
- [gen_js_api: easy OCaml bindings for JavaScript libraries](https://github.com/LexiFi/gen_js_api)
- [Writing JavaScript using OCaml](https://www.kuniga.me/blog/2018/06/24/writing-javascript-using-ocaml.html)
- [Confused summary of history of BuckleScript](https://rescript-lang.org/blog/bucklescript-is-rebranding#history--summary)
- [Confused about ReScript? ReScript, Reason, ReasonML, and BuckleScript explained](https://ersin-akinci.medium.com/confused-about-rescript-rescript-reason-reasonml-and-bucklescript-explained-ab4230555230)
- [js_of_ocaml vs BuckleScript](https://discuss.ocaml.org/t/js-of-ocaml-vs-bucklescript/2293/8)
- [ReasonML vs BuckleScript](https://medium.com/lambdaside/reasonml-vs-bucklescript-7bca6eae7730)

### Learning React 

- [React -- Quick start](https://react.dev/blog/2023/03/16/introducing-react-dev#quick-start)