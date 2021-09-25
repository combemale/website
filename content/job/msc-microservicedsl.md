+++
title = "Internship: Towards Polyglot Code Refactoring"
date = 2021-08-01
math = false
highlight = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = ""
caption = ""

+++

## keywords
Programming Language, Software Language Engineering, Domain-Specific Language, Polyglot Development, Integrated Development Environment, Refactoring, Co-evolution, Code Repair. 

## Context and Challenges

The evolution of software engineering discipline has seen the emergence of a multitude of programming languages (PL), each dedicated to a particular application concern. Nowadays, complex software development often involves more than a single language for the implementation, referred to as polyglot development . Indeed, we observe more and more software projects that are implemented with various PLs, in particular, to combine their strengths and counterbalance their weaknesses. For example, polyglot development is relevant and popular in development of web applications, video games, DSLs, etc. Emerging solutions do exist that support polyglot programming relying on Intermediate Representation (IR), such as the GrallVM/Truffle, PolyNote notebook, LLVM, or WebAssembly.

While polyglot development allows developers to choose the appropriate language to implement a given concern, it also leads to a set of loosely coupled (i.e., with data sharing through variables and functions calls) and heterogeneous programs difficult to globally reason over them. Indeed, the existing frameworks do not reify the relationships between them and poorly support the developers on the global impact (i.e., in other programs) of any code change. 

## Objectives

The main objectives of this internship are the following: 
1. state of the art on semantic-preserving refactorings, co-evolution and code repair, experimented on specific languages ;
1. complement the catalog of semantic-preserving refactorings to cover polyglot development scenarios ;
1. Propose a unifying development framework to convey any code change over the overall heterogeneous programs, and analyse the global consistency ;
1. develop a prototype that automates the application of polyglot semantic-preserving refactorings in reaction to code changes to ensure the global consistency of the overall software system.

This internship will be done in the context of international collaboration between DiverSE/IRISA and CWI through the international ALE team, and with our contact in ORACLE (GrallVM/Truffle). 

## Required and appreciated skills

- strong skills in programming, more specifically, fluent in object-oriented programming ;
- passionate about programming languages, language theory, language design & implementation and integrated development environment ;
- autonomy, and excellent English speaking and writing skills.

## Environment

The candidate will work in the DiverSE team, common to CNRS (IRISA) and Inria. The DiverSE team is located in Rennes, France. DiverSE’s research is in the field of software engineering. The team is actively involved in European, French and industrial projects and is composed of 9 professors/researchers, 20 PhD students, 4 post-docs and 3 engineers. The main supervisors of the thesis will be Benoit Combemale (benoit.combemale@irisa.fr) and Djamel Khelladi (djamel-eddine.khelladi@irisa.fr). 

## References

- Fabio Niephaus et al.. “Example-Based Live Programming for Everyone: Building Language-agnostic Tools for Live Programming with LSP and GraalVM”, Onward! 2020 
- McDirmid, Sean. “Usable live programming”, Onwards! 2013 
- Santolucito, Mark, William T. Hallahan, and Ruzica Piskac. “Live programming by example.” In Extended Abstracts of the CHI 2019 
- Hidehiko Masuhara, Shusuke Takahashi, Yusuke Izawa, Youyou Cong. “Toward a Multi-Language and Multi-Environment Framework for Live Programming”, LIVE 2020. 
- Würthinger, Thomas, et al. “One VM to rule them all”, Onward! 2013 
- Niephaus, Fabio, Tim Felgentreff, and Robert Hirschfeld. “GraalSqueak: toward a smalltalk-based tooling platform for polyglot programming” In Proc. of MPLR 2019 
- Niephaus, Fabio, Tim Felgentreff, and Robert Hirschfeld. “Towards polyglot adapters for the graalvm” In Proc. of Programming 2019.