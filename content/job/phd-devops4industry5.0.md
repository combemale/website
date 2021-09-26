+++
title = "PhD Thesis: DevOps for Industry 5.0."
date = 2021-08-01
math = false
highlight = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = ""
caption = ""

+++

## Context

The design of complex cyber-physical systems (e.g., industry 5.0) involves various heterogeneous stakeholders (e.g., software engineers, computer and system engineers, mechanical engineers, physicists), all bringing their own expertise to the system, and for this using their own tools and methods. The disruptive design of new, complex systems requires a high degree of flexibility in the communication between these many stakeholders, often limited by the siloed structure of the organization itself (cf. Conway's law). To overcome this constraint, modern engineering environments aims to: better manage the necessary exchanges between the different stakeholders; provide a unique place for information sharing; ensure the consistency of the many points of view. Beyond these classical goals,  they also aim at handling value streams, which are characterized by partial orders of activities that require either a social (i.e., among the stakeholders) or a technical (i.e., among the artefacts) coordination.  Providing a unifying framework for managing these various activities will ​allow breakthrough innovations and the search for global optimum. 

The first generations of these engineering environments made it possible to understand the specificities of each stakeholders by allowing them to use their own formalisms (aka. domain-specific modeling languages), while maintaining the overall consistency and the ability to think globally about the system being designed through an holistic digital representation. These environments are sometimes also backed by a methodology to guide the process of creating different points of view. However, these methodologies remain independent of the value stream ​​passing between the many stakeholders involved in the process. This limitation affects the ability to establish a collective intelligence where all individuals collaborate globally and in an agile manner. For this, a correctly identified, transparent value stream, equipped with suitable and partially automated tools to facilitate its handling is essential to promote the creativity necessary in the design phase, while enhancing the involvement of everyone.

To overcome this limit to collective intelligence when designing complex systems, this thesis aims to improve the usability of development cycles, involving both systems engineers and all those involved in specialty engineering. Usability will be approached through three complementary aspects:
- Efficiency, which aims to achieve a result with less effort,
- Affordance, in particular perceptible affordance, which is the ability of an object to suggest its uses,
- Satisfaction, which is the comfort of the user in using the engineering environment and performing tasks.

## Objective

To improve the usability (in its three facets) of the development of complex systems, we propose to leverage on modern software engineering practices such as DevOps and web-based collaborative platforms (e.g., forges). DevOps aims, among other things, to reduce the distance between the different stakeholders (esp., developpers and IT) and to improve interactions between them thanks to an adapted tool chain. The execution of this tool chain aims to produce an overall result as quickly as possible (software, data, etc.). The search for this overall result brings together the various stakeholders involved, possibly coming from different fields, around a common final objective. In the context of systems engineering, DevOps would take advantage of the established value stream to automate certain activities as much as possible, and ensure continuous improvement on the system being designed. Forges (e.g., Gitlab, GitHub) are web-based collaborative platforms that bring all stakeholders in a virtual common place to realize the value stream in software development.

While such practices had a deep impact in the software engineering community in the last decade, there are many scientific and technical obstacles to apply them more widely to all the stakeholders involved in the design of complex systems:
- How to establish a main chain of DevOps tools for systems engineering seeking global optima through socio-technical coordination of the different stakeholders involved?
- How on a local chain of DevOps tools can a stakeholder rely to study local optima without affecting the main chain?
- How, in a DevOps context, can an evolution carried out by a stakeholder on his data propagate to other impacted data managed by other stakeholders?
- How to notify a stakeholder in case of detection of an impact on his data so that he can benefit easily and quickly from these changes?
- How a multi-disciplinary pull request can be implemented to support the required socio-technical coordination? 
- How can each stakeholder, with their specific point of view, visualize, validate and analyze local and global optima?

The work will be applied and evaluated in the field of industry 5.0, which not only considers producing goods and services for profit, but also making it sustainable, human-centric and resilient. All these concerns have to be considered by design, and involve various heterogeneous stakeholders and artefacts to be intelligently coordinated. 


## Environment

Le candidat travaillera dans l'équipe DiverSE, commune au CNRS (IRISA) et à Inria. L'équipe DiverSE est située à Rennes. Les recherches de l'équipe DiverSE se situent dans le domaine du génie logiciel. L'équipe est activement impliquée dans des projets européens, français et industriels et est composée de 9 enseignants-chercheurs, 20 doctorants, 4 post-docs et 3 ingénieurs. Les tavaux de thèse seront dirigés par [Arnaud Blouin](https://people.irisa.fr/Arnaud.Blouin/) (INSA, DiverSE team), [Benoit Combemale](https://people.irisa.fr/Benoit.Combemale) (University of Rennes 1, DiverSE team) et [Djamel Eddine Khelladi](http://people.irisa.fr/Djamel-Eddine.Khelladi/) (CNRS, DiverSE team). Le candidat s'inscrira à l'école doctorale en informatique de l'Université de Rennes 1.