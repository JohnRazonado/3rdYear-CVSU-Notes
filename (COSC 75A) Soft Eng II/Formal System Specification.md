> #inProgress 
## Formal Technique
- Mathematical method  to specify hardware and/or software system
- Verify that specification is realizable, implementation satisfies its specification, prove properties of system, etc.

## Formal Specification Language
- Consists of two sets: **syn and sem,** and **relation sat**
- **syn** = Syntactic domain
- **sem** = Semantic domain
- **relation sat** = satisfaction relation

## Syntactic Domains
- Consists of alphabet of symbols and set of formation rules to construct well-formed formulas from the alphabet.
- From the term, syntax. mostly controls what variables, rules, and organization is used to form the formula.

## Semantic Domains
- Many formal techniques use different semantic domains
- Abstract data type specification languages - algebras, theories, and programs
- Programming languages - specify functions to input and output values.
- Concurrent and distributed system specification languages - state sequences, event sequences, state-transition sequences, synchronization trees, partial orders, state machines, etc.
## Satisfaction Relation
- Its important to determine the element of semantic domain satisfies the specifications.
- Satisfaction is determined by a homorphism as **"semantic abstraction function"**. 
	- Maps elements of the semantic domain into equivalent classes.
	- two broad classes: **preserve a system's behavior** and **preserve a system's structure**.

## Model-oriented vs. Property-oriented Approaches

### Model-oriented
- defines system's behavior directly by constructing model of system in terms of mathematical structures.
- suited to use in later phases of life cycle
- use logical operations but don't support conjunction (AND) and disjunctions (OR)

### Property-oriented
- System's behavior defined indirectly by stating its properties, usually in form of sets of axioms.
- suitable for requirements specifications since they can be easily changed.
- Sample are specification styles of axiomatic specification and algebraic specification.

## Operational Semantics
- Way of computations are represented
- There are a lot of types:

### Linear Semantics
- Run of system described by a sequence (possible infinite) of events or states.
- represented by non-deterministic interleavings of the automatic actions.

### Branching Semantics
- Behavior of a system is represented by directed graph.
- nodes of graph - possible staes in the evolution of system
- descendants of each nodes - states of atomic actions enabled at that state.
### Maximally parallel semantics
- Concurrent actions enabled at any state are assumed to be taken together 

### Partial order semantics
- Semantics to a system is a structure of states satisfying partial order relation among states (events).
- Represents precedence ordering among events and constraints some events.
## Positive features of Formal methods
- **Encourage rigor** - very process of construction of a rigorous specification is more important then formal specification itself.
- **Well-founded mathematical basis** - not only more precise but mathematically sound and can be used to reason about the properties of specification.
- **Well-defined semantics** - ambiguity in specifications is automatically avoided
- **Automating analysis of specifications** - automatic theorem proving techniques can be used to verity that an implementation satisfies its specifications. 
- **Obtain immediate feedback on the features** - Concept of *executable specifications* is related to rapid prototyping. Useful in checking completeness of specifications

## Limitation of Formal Requirements Specification
- Difficult to learn and use
- Impossible to check absolute correctness of system using theorems
	- Due to basic incompleteness results of first-order logic
- Not able to handle complex problems - even moderately complicated problems blow up the complexity of formal specification.

## Axiomatic Specification
- first-order logic used to write pre and post- conditions.
- pre-condition - capture conditions that must be satisfied before an operation can be successfully invoked.
- post conditions - must be satisfied when function completes execution for function to be considered fully executed.

### Steps to follow axiomatic specifications of function:
- Establish range of input values
- Specify predicate defining conditions 
- Establish changes made to the function's input parameters after execution of function.
- Combine all of the above into pre and post conditions.

### Example 1


### Example 2
