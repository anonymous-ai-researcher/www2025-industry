## Environment requirement

* JDK 1.8
* IDE: IDEA 
* Maven

## Import of this project

* Unzip this project.
* Import it into IDEA.
* Make the src folder as source root.
* Make sure that the jar package under the root folder has been added into project as libriaries.

## Description of the UI tool

* The UI tool is a high-performance prototype for computing uniform interpolants of **ELIH-Ontologies**. It can be used as a Java library or a standalone tool for UI and related tasks.

* A uniform interpolant provides a restricted view of an ontology using only a subset of its signature (the interpolation signature) while preserving all logical entailments over this subset in the absence of other names from the original signature. It can be computed by incrementally forgetting names outside the interpolation signature—collectively forming the complementary forgetting signature—while maintaining all logical entailments expressible in the interpolation signature.

* If an input ontology is not an ELIH one, our tool simply takes the ELIH fragment of the ontology and discards those axioms not expressible in ELIH. If an input ontology contains cyclic dependencies over the names in the forgetting signature, the result cannot always be represented finitely without fixpoint operators. Since fixpoint operators are not supported by OWL API, our UI tool introduces additional concept names, namely definers, to the output ontology that simulate the behaviour of fixpoint operators. In this sense, the result is no longer a uniform interpolant, since it contains extra names that are not in the specified interpolation signature.

## Run of the UI tool

* To run the forgetting method, go to  **/src/forgetting/Forgetter.class** and call the method: 

  ```java
  public Set<OWLAxiom> ForgettingAPI(Set<OWLObjectProperty> roles, Set<OWLClass> concepts, OWLOntology onto)
  ```

* The input are a set of role names to be forgotten  ( ``` Set<OWLObjectProperty> roles ``` ),  a set of concept names to be forgotten ( ``` Set<OWLClass> concepts ``` ) and an ELIH-Ontologies from which the concept and role names are forgotten ( ``` OWLOntology onto ``` ).

* The output is another ELIH-Ontology which is a uniform Σ-interpolant of the ontology ``onto``, represented as a set of OWLAxioms.

* An example illustrating the usage of the UI tool is included in the Forgetter.class main function.

## Run of the OntoLdiff tool

* To run the logical difference detection method, go to /src/forgetting/LDiff.java and call the method: 

  ```java
  public void compute_LDiff(OWLOntology onto_1, OWLOntology onto_2, String path)
  ```

* The input are two ELIH-ontologies to be compared (onto_1, onto_2), and a path specifying the location where you want the output to be saved. The output are a set of witnesses, a set of explicit witnesses (contained) and a set of implicit witnesses (derived), saved as owl.xml files; see the following example (please adjust it to your own operating environment, i.e., windows, linux or Mac).

* Onto_1: file:///C:/Users/XXX/Desktop/snomed_ct/snomed_ct_australian.owl

* Onto_2: file:///C:/Users/XXX/Desktop/snomed_ct/snomed_ct_intl_20170731.owl 

* Path: C:\Users\XXX\Desktop\snomed_ct
