+++
title = "Internship: From Monolithic to Microservice Architecture: The Case of Extensible and Domain-Specific IDEs"
date = 2020-08-01
math = false
highlight = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = ""
caption = ""

+++

## keywords
Microservice, DevOps, Domain-Specific Languages

## Context and Challenges

The software engineering community recently introduced the concept of microservice [1] as a support for a new distributed and dynamic software architecture. Microservices are orchestrated, self-contained, reusable and minimalist processes interacting via messages. This new software architecture enables complex applications to be more readable and maintainable, together with a better quality of service with scalability and dynamic reconfiguration. Both academy and industry investigated new tools and methods to support software development following this new architecture (e.g., microprofile, Quarkus/SpringBoot, Kubernetes/Nomad, etc). In practice, this new software architecture has been instrumental in the development of large-scale applications with complex and varying contracts of quality of services, such as Netflix [2], Spotify [3], and Uber [4].

However, the success of such an architecture in large applications lead to an increasing number of microservices that comes with new challenges. In particular, the developer needs to provide complex orchestrators, and faces complex deployment and delivery pipelines over very heterogeneous technologies (e.g., various execution platforms, communication protocols, etc.).

## Objectives

During this internship, we propose to explore the definition of an environment that supports the developper in the task of specifying, orchestrating, and deploying complex applications based on microservices. The main objective is to identify the relevant abstractions for the developper within domain-specific languages [5,6], and to define the required generative approaches to leverage on the diversity of the available technologies.

As a case study, we propose in this internship to focus on Integrated Development Environments (IDEs). Modern IDEs are complex software that offers a wide variety of very heterogeneous services (workspaces, syntax checking, autocompletion, debugging, ...). Depending on the language, its use, and the available environment, the set of available services might change to provide a more tailored experience, and it is essential to support the required workflows that correspond to the different usages.

## Description of the Work

The candidate will first perform a literature review on both microservice definition and orchestration, and the recent practices in IDE development (e.g., protocols like LSP and DAP). This body of knowledge will be used as a basis for identifying the relevant abstractions to be implemented in the form of domain-specific languages. Such a domain-specific language will be complemented with the required geenrative appraoch to automate the modularisation, deployment and dynamic reconfiguration of software applications based on microservices.  

In the context of this internship, the candidate will work more specifically on IDEs, and will propose an approach to modularize and orchestrate environment-agnostic language features in IDEs (in a similar fashion to Microsoft VSCode's language services but with additional concerns of distribution, scalability and reconfiguration) according to an architecture based on microservice.

## Required and appreciated skills

- English language proficiency
- Autonomy, communications skills, and desire to work in a team environment
- Expertise in object-oriented development
- Strong interest in programming languages and language engineering
- Experience in the development of IDE components will be a plus

## Environment

The candidate will work at Inria in the DiverSE team. Inria is the French national institute for research in computer science. There are 8 Inria research centres located throughout France, hosting more than 200 research teams. The DiverSE team is located in Rennes. DiverSE’s research is in the area of software engineering. The team is actively involved in European, French and industrial projects and is composed of 9 faculty members, 20 PhD students, 2 post-docs and 4 engineers. The candidate will work in the context of one of the main topic currently explored in the team, involving various professors and students. The main supervisors will be Prof. Benoit Combemale and Prof. Olivier Barais (University of Rennes 1, DiverSE team), as well as Pierre Jeanjean, a PhD student currently exploring some related challenges.

## References

1. J. Thones. “Microservices”. In: IEEE Software 32.1 (2015), pp. 116–116. doi: 10.1109/MS.2015.11.
2. M. McGarr, E. Bukoski, and B. Moyles. How We Build Code at Netflix. 2016. url: http://techblog.netflix.com/2016/03/how-we-build-code-at-netflix.html.
3. How We Use Backstage at Spotify. 2020. url: https://engineering.atspotify.com/2020/04/21/how-we-use-backstage-at-spotify/.
4. Einas Haddad. Service-Oriented Architecture: Scaling the Uber Engineering Codebase As We Grow. 2015. url: https://eng.uber.com/service-oriented-architecture/.
5. Benoit Combemale et al. Engineering Modeling Languages: Turning Domain Knowledge into Tools. Chapman and Hall/CRC, Nov. 2016, p. 398. url: http: //mdebook.irisa.fr/
6. Douglas C. Schmidt. “Guest Editor’s Introduction: Model-Driven Engineering”. In: Computer 39.2 (Feb. 2006), pp. 25–31. issn: 0018-9162. doi: 10.1109/ MC.2006.58. url: https://doi.org/10.1109/MC.2006.58.