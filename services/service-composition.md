#Service Composition

- A service composition combines services following a certain composition pattern to achieve a business goal,
solve a scientific problem, or provide new service functions in general (Curbera, Khalaf, Mukhi, Tai, &
Weerawarana, 2003)

- Service compositions may themselves become services, making composition a
recursive operation.

- During an online order process for example, a composition can exist of a service that
checks a customer’s zip code as well as the delivery time of the goods ordered.

##Approaches for service composition

###BPEL4WS

BPEL4WS is an abbreviation of Business Process Execution Language for Web Services. It is often
shortened to ‘BPEL’. It is an XML based orchestration language, standardized by the Organization for the
Advancement of Structured Information Standards (OASIS). BPEL supports a process-oriented form of
service composition (Curbera, Khalaf, Mukhi, Tai, & Weerawarana, 2003). Process orientation denotes that
each BPEL composition is a business process or workflow that interacts with a set of Web services to
achieve a certain goal (Curbera, Khalaf, Mukhi, Tai, & Weerawarana, 2003).

A BPEL composition interacts with a set of web services to achieve a given task (Milanovic & Malek, 2004).
In BPEL the composition result is called a process, participating services are partners, and message
exchange or intermediate result transformation is called an activity (Milanovic & Malek, 2004).

###OWL-S

OWL-S is a part of the Semantic Web vision (Milanovic & Malek, 2004). OWL-S is an ontology built on top of
Web Ontology Language (OWL) by the DARPA DAML program. It replaces the former DAML-S ontology
(http://www.w3.org/Submission/OWL-S/) OWL-S is a services ontology that enables automatic service
discovery, invocation, composition, interoperation and execution monitoring (Milanovic & Malek, 2004).
Using OWL-S the composition process can be executed without human involvement.

This approach treats services as components, a web component packages together elementary or complex
services and presents their interfaces and operations in a consistent and uniform manner in the form of a
class definition (Yang & Papazoglou, 2002). The main idea is to encapsulate composite-logic information
inside a class definition, which represents a web component (Milanovic & Malek, 2004). A web component’s
public interface can then be published and used for discovery and reuse (Milanovic & Malek, 2004). Web
components support basic software development principles as reuse, specialization and extention (Yang &
Papazoglou, 2002).


###π-calculus

π-calculus is an algebraic method to describe processes, π-calculus is described by Milner (Milner, 1991). In
π-calculus the basic entity is a process, types of process are an empty process, a choice between several
I/O processes and their continuations, a parallel composition, a recursive definition or a recursive invocation
(Milanovic & Malek, 2004). IO operations can be input (receive) or output (send). When compositions are
described using pi-calculus it is possible to reason about composition correctness (Meredith & Bjorg, 2003).


###Petri net

A Petri net is a directed, connected and bipartite graph in which nodes represent places and transitions and
tokens occupy places (Milanovic & Malek, 2004). When there is at least one token in every place connected
to a transition, that transition is enabled (when modeling web services this would mean it is possible to
invoke a web service because all input requirements are met). An enabled transition might fire by removing
one token from every input place, and depositing one token in each output place (Milanovic & Malek, 2004).


###Model checking

Model checking is used to formally verify finite-state concurrent systems. In case of model checking, the
system specifications are described using temporal logic, then the model is used (traversed forward and
back) to determine whether the specification holds (Maximilien & Singh, 2004).