+++
# Date this page was created.
date = "2017-10-19"

# Name.
name = "SLE"
title = "Software Language Engineering"
from = "2020-08-01"

# Optional external URL for project (replaces project detail page).
# external_link = "#"

# Tags: can be used for filtering projects.
tags = ["course"]

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = ""
caption = ""

+++

<h4><a title="Benoit Combemale's Homepage" href="https://www.irit.fr/~Benoit.Combemale/" target="_blank">Benoit Combemale</a> (Univ. Toulouse & Inria)</h4>

## Description
Software engineering faces new challenges with the advent of modern software-intensive systems such as complex critical embedded systems, cyber-physical systems and Internet of things. Application domains range from robotics, transportation systems, defense to home automation, smart cities, and energy management, among others. Software is more and more pervasive, integrated into large and distributed systems, and dynamically adaptable in response to a complex and open environment. As a major consequence, the engineering of such systems involves multiple stakeholders, each with some form of domain-specific modeling.

Model-Driven Engineering (MDE) aims at reducing the accidental complexity associated with developing complex software-intensive systems through the use of modeling techniques that support separation of concerns and automated generation of system artifacts from models. Separation of concerns is founded on the exploitation of different domain-specific <em>modeling</em> languages (DSLs), each providing constructs based on abstractions that are specific to a concern of a system. As such, DSLs are “the heart and soul” of MDE, and have major consequences on the industrial development processes.

The integration of domain-specific concepts and best practices development experience into DSLs can significantly improve software and systems engineers productivity and system quality. For such a purpose, the development of DSLs has been recently recognized as a significant software engineering task itself. Indeed, the development of DSLs is a challenging task which requires specialized knowledge. This recently resulted in the emergence of Software Language Engineering (SLE), defined as the application of systematic, disciplined, and measurable approaches to the development, use, deployment, and maintenance of software languages.

This course provides an end-to-end coverage of the engineering of modeling languages to turn domain knowledge into tools. It introduces the foundations of SLE, with a specific focus on the use of modeling techniques for designing and implementing DSLs. It also provides various illustrations through the definition of different kinds of modeling languages, their instrumentation with tools such as editors, interpreters and generators, the integration of multiple modeling languages to achieve a system view, and the validation of both models and tools.

The course starts with definitions of modeling and MDE, and then moves into a deeper discussion of how to express the knowledge of particular domains using modeling languages to ease the development of systems in the domains. The second part presents examples of applications of the model-driven approach to different types of software systems. In addition to illustrating the unification power of models in different software domains, this part demonstrates applicability from different starting points (language, business knowledge, standard, etc.) and focuses on different software engineering activities such as Requirement Engineering, Analysis, Design, Implementation, and V&V.

## Textbooks

<p style="text-align: center;"><a href="http://mdebook.irisa.fr/" title="Textbook on MDE and SLE (CRC Press, 2017)" target="_blank"><img class="wp-image-1464" style="border: 0px;" src="../../img/MDEBook_cover-1.jpg" width="115" /></a></p>

## Lectures (Materials)

<ul>
	<li><a href="#">From MDE to SLE</a></li>
	<li><a href="#">Pragmatics of SLE</a></li>
	<li><a href="#">Domain-Specific Languages: Basics</a></li>
	<li><a href="#">Domain-Specific Languages: Advanced (staging, att. grammars, typing, op. semantics...)</a></li>
	<li><a href="#">Language workbenches</a></li>
	<li><a href="#">Program and model transformation (static analysis, code/test/doc generation...)</a></li>
	<li><a href="#">Program and model execution, simulation and debugging</a></li>
	<li><a href="#">Program and model composition (merge, coordination, synchronization)</a></li>
</ul>

## Further Materials

- Language workbenches
- SLE conference
- SLEBoK
- DSL book (ralf)