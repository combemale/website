+++
title = "Internship: Towards Distributed and Scalable IDE."
date = 2021-08-01
math = false
highlight = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = ""
caption = ""

+++

## Context and objectives

Integrated Development Environments (IDEs) are indispensable companions to programming languages. They are increasingly turning towards Web-based infrastructure. The rise of protocols such as the Language Server Protocol (LSP) that standardize the separation between a language-agnostic IDE, and a language server that provides all language services (e.g., auto completion, compiler...) has allowed the emergence of high quality generic Web components to build the IDE part that runs in the browser. Protocols allow language servers to be reused accross different IDEs, and web-based interfaces facilitate access to the IDE.

Beyond these first benefits, web-based IDEs also open up new perspectives in terms of collaborative environments, both for general-purpose languages and domain-specific languages. However, this requires all language services to be well identified and to scale according to their use. 

In contrast with the current approaches that provide IDEs in the form of a monolithic client-server architecture, we propose to investigate the modularization of the various languages services, and the definition of a specific protocol between them to support their individual deployment, and possible dynamic reconfiguration according to their use. 

## Description of the work

After a review of the literature and the state of practices regarding the recently introduced protocols, the student(s) will:
- propose a systematic approach to modularize the various language services, and establish a protocol between them to suport their communication. In particular, the protocol will have to manage the shared ressources, e.g., the programs available in the workspace.
- a generative approach to automate the deployment or dynamic reconfiguration of the vraious services accross the available execution platform, and according to the defined protocol and current context. 
- a predictive model to capture the environment and the runtime data of the various language services, and recommend the best configuration of the deployment according to the current context.

## Environment

The candidate will work at Inria in the DiverSE team. Inria is the French national institute for research in computer science. There are 8 Inria research centres located throughout France, hosting more than 200 research teams. The DiverSE team is located in Rennes. DiverSE’s research is in the area of software engineering. The team is actively involved in European, French and industrial projects and is composed of 9 faculty members, 20 PhD students, 2 post-docs and 4 engineers.
The candidate will work in the context of one of the main topic explored in the team, involving various professors and students, as well as a close partnership with CWI in Amsterdam. The main supervisors will be Prof. Benoit Combemale and Prof. Olivier Barais (University of Rennes 1, DiverSE team).




