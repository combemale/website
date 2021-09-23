+++
# Date this page was created.
date = "2021-01-01"

# Name.
name = "Master ICE, 1st year"
title = "Course materials for students of the 1st year of the Master ICE"
from = "2021-01-01"

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

# ICE1-IDM: hack your own language

The course introduces the state-of-the-art tools and methods for developping domain-specific languages.

## Lectures
**Professor**: [Benoit Combemale](https://people.irisa.fr/Benoit.Combemale)

- [Model-Driven (software) Engineering: Hack your Own Language!](../../pub/course/sle/2021-SLE-1-intro.pdf)
- [Domain-Specific Languages](../../pub/course/sle/2021-SLE-2-dsl.pdf)
- [Model Management](../../pub/course/sle/2021-SLE-3-ModelManagement.pdf)
- [Model Execution](../../pub/course/sle/2021-SLE-4-ModelExecution.pdf)

## Textbooks

<p style="text-align: center;"><a href="http://mdebook.irisa.fr/" title="Textbook on MDE and SLE (CRC Press, 2017)" target="_blank"><img class="wp-image-1464" style="border: 0px;" src="../../img/MDEBook_cover-1.jpg" width="115" /></a>  &nbsp;&nbsp;<a href="http://www.amazon.fr/Ing%C3%A9nierie-Dirig%C3%A9e-par-Mod%C3%A8les-concepts/dp/2729871969" target="_blank" title="[French] Manuel sur l'IDM (Ellipses, 2012)"><img class="wp-image-1467" style="border: 0px;" src="../../img/LivreIDM_ombre-251x300.png" alt="livreidm_ombre" width="155" /></a></p>

## Labs
**Professor**: [Benoit Combemale](https://people.irisa.fr/Benoit.Combemale)

The labs will consist in realizing by group of 2 the following tutorial. The evaluation will consist in a final demonstration on Thursday, Feb. 4th, 16h-18h.

### Overall objectives of the labs

The main objective of this tutorial is to build your own state-machine language (aka. FSM, standing for _Finite State Machine_), including the design of the domain (i.e. concepts and relationships between them), and the developement of the associated tooling: a textual editor, a compiler (to Java code), and an interpreter. 

With FSM, we expect to be able to model a state machine according to the textual syntax proposed in the following example, through a modern editor (e.g., syntax highlighting, autocompletion, validation rules and quick fixes, code folding...): 
	
~~~~
fsm door
    state opened entry "open door" 
    state init closed entry "close door"
    transition open closed -> opened [on]
    transition close opened -> closed [off]
~~~~

A model (e.g., _door_) conforming to your language (aka., _FSM_), can then be executed, either through a compilation (i.e. code generation) to a Java-based implementation, or through a direct interpretation (i.e., virtual machine). 

For the execution, input events (e.g., _on_ and _off_) that drive the execution can be injected through the console by the user. 

> The proposed _FSM_ language to be designed and implemented is a simple automata. Automata are a core paradigm for MANY domain-specific languages used in practice, either for high level design (e.g., functional chains in systems engineering), analysis (e.g., termination, composability, etc.), or development (e.g., agent based simulations, reactive programming, etc.). 

### Part 1 - Domain modeling: definition of the Ecore metamodel for your language

The main objective of this part is to capture in an Ecore metamodel the concepts and relationships between them of the domain addressed by your language (i.e. the domain of state machine). You are expected to identify the required concepts to model the aforementionned example, and to reify them into language constructs, in the form of a metamodel defined with the metalanguage Ecore and the associated tooling (e.g., graphical editor), aka. Ecore tools. 

Within your Eclipse RCP that includes EMF, Xtext and Xtend (e.g., the GEMOC Studio), create an _Ecore Modeling Project_. Give a proper name to your project (e.g., _fr.ice.fsm.model_) and your package (e.g., _fsm_).

From this point, you can start model your domain in the form of an object-oriented metamodel consisting of classes and relationships between them. 

You may validate your metamodel by right click on your ecore model and _Validate_.

When this is done, you can generate the Java-based implementation of your domain model by opening the associated genmodel file, right click on the root element and _Generate all_

You may assess the expressivity of your metamodel (i.e., check if it well captures your domain, in your case meaning it supports the modeling of the proposed example) by opening the ecore metamodel, right clic on the concept of the root element of your expected model, and choose _Create dynamic instance_. Then you can create a model in a tree-based editor, and ensure your metamodel supports the expected model structure. 

### Part 2 - Textual modeling: definition of the Xtext editor for your language

The next step consists into going further than the tree-based editor by developing a modern textual editor. You will use Xtext for this purpose.

Create a new _Xtext Project From Existing Ecore Models_, select the genmodel file associated to your Ecore metamodel, and select the concept of the root element (i.e., the first model element that will be instantiated when you will create a new model). 

Take care of properly filling-in the wizard. Then Xtext provides you a first version of a grammar for the textual syntax of your language. 

> You may need to add the Xtext nature to the project where is your Ecore metamodel to make sure the Xtext project can compile (right clic on the project, _configure_ and _add Xtext nature_). 

You can immediatly start a new eclipse from the current one (_Run configuration..._ > _Eclipse Application_), create a new empty project and a blank file with the choosen extension. Eclipse will propose you to open it with the corresponding Xtext editor, and then you can use it according to the syntax proposed by the automatically generated grammar. 

Modify your grammar to make sure you can model a state machine according to the syntax proposed in the initial example. You may also have a try to the following example :)

~~~~
fsm door
    state opened entry "open door" 
    state init closed entry "close door"
    transition open closed -> opened [on]
    transition close opened -> closed [off]
    state broken entry "broken door"
    transition b1 opened -> broken [warning]
    transition b2 closed -> broken [warning]
~~~~

### Part 3 - Compilation: definition of the Xtend-based compiler for your language

Up to now, you identified the concepts of your language (which set its expressivity) and you implemented a textual editor to support the edition of conforming models (_aka._ programs). The next step is the ability of executing such models. For this purpose, there are two possibilities: by compilation (_aka._ code generation) to an executable implementation, or by interpretation (_aka._ virtual machine). 

In this part of the tutorial, we ask you to complement your metamodel with the implementation of an Xtend-based compiler, following the design pattern [visitor](https://refactoring.guru/design-patterns/visitor). In the case of FSM, such a compiler must generate a Java-based implementation of a given model (i.e., a state machine) according to the design pattern [state](https://refactoring.guru/design-patterns/state). 

Votre compilateur peut avoir comme point d'entrée [la méthode _doGenerate_](https://www.eclipse.org/Xtext/documentation/103_domainmodelnextsteps.html) de la classe _fr.ice.fsm.generator.FsmGenerator_ pour être appelé à chaque sauvegarde d'un modèle édité avec l'éditeur textuel développé avec Xtext dans la partie précédente.  

### Part 4 (optional) - Interpretation: definition of the Xtend-based interpreter for your language

In this part, we ask you to develop a new visitor that will interpret a given conforming model instead of generating an implementation in a third party language (i.e. Java in the case of the compiler developped in the previous part). Similarly to a compiler, an interpreter goes through the asbtract syntax tree of a given model. Instead of generating the corresponding code, it interprets the model element in terms of changes in a model state (aka., _context_). This is captured in an additional design pattern called [interpreter](https://en.wikipedia.org/wiki/Interpreter_pattern) that can be used to complement the design pattern [visitor](https://refactoring.guru/design-patterns/visitor).

## Further material

- The [Refcardz on EMF](https://dzone.com/refcardz/essential-emf)
- Documentations of [Xtext](https://www.eclipse.org/Xtext/documentation/) and [Xtend](https://www.eclipse.org/xtend/documentation/index.html)
- [The GEMOC Studio](http://gemoc.org/studio.html) (incl., EMF, Xtext, Xtend, Sirius...)