```diff
- Please find above an extended version of the paper including all missing proofs and the empirical results.

- Some typographical errors in the original text are corrected here:
- Original Text:
- Page 2: This paper focuses on the computation of syntax-restricted modules...
- Page 3: Uppercase letters A and B denote concept names. Uppercase letters C and subsequent letter in the alphabet represent general concepts.

- Corrected Text:
- Page 2: This paper focuses on the computation of signature-restricted modules...
- Page 3: Uppercase letter A denotes concept names. Uppercase letters B, subsequent letters in the alphabet, and the Greek letters Φ and Ψ denote general concepts.
```
## Environment requirement

* JDK 1.8
* IDE: IDEA 
* Maven

## Data

* Statistics of Oxford-ISG & BioPortal (Min:Minimum, Max:Maximum, Med:Medium, 90 Ptl: 90th Percentile):


<div align="center">
<table class="tg">
<thead>
  <tr>
    <th class="tg-7btt" colspan="2">Oxford</th>
    <th class="tg-7btt">Min</th>
    <th class="tg-7btt">Max</th>
    <th class="tg-7btt">Med</th>
    <th class="tg-7btt">Mean</th>
    <th class="tg-7btt">90Ptl</th>
    <th class="tg-7btt">%</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow" rowspan="3">I</td>
    <td class="tg-c3ow">|N<sub>C</sub>|</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-c3ow">1582</td>
    <td class="tg-c3ow">86</td>
    <td class="tg-c3ow">191</td>
    <td class="tg-c3ow">545</td>
    <td class="tg-c3ow">n/a</td>
  </tr>
  <tr>
    <td class="tg-c3ow">|N<sub>R</sub>|</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-c3ow">332</td>
    <td class="tg-c3ow">10</td>
    <td class="tg-c3ow">29</td>
    <td class="tg-c3ow">80</td>
    <td class="tg-c3ow">n/a</td>
  </tr>
  <tr>
    <td class="tg-c3ow">|Onto|</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-c3ow">990</td>
    <td class="tg-c3ow">162</td>
    <td class="tg-c3ow">262</td>
    <td class="tg-c3ow">658</td>
    <td class="tg-c3ow">82.20</td>
  </tr>
  <tr>
    <td class="tg-c3ow" rowspan="3">II</td>
    <td class="tg-c3ow">|N<sub>C</sub>|</td>
    <td class="tg-c3ow">200</td>
    <td class="tg-c3ow">5877</td>
    <td class="tg-c3ow">1665</td>
    <td class="tg-c3ow">1769</td>
    <td class="tg-c3ow">2801</td>
    <td class="tg-c3ow">n/a</td>
  </tr>
  <tr>
    <td class="tg-c3ow">|N<sub>R</sub>|</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-c3ow">887</td>
    <td class="tg-c3ow">11</td>
    <td class="tg-c3ow">34</td>
    <td class="tg-c3ow">61</td>
    <td class="tg-c3ow">n/a</td>
  </tr>
  <tr>
    <td class="tg-c3ow">|Onto|</td>
    <td class="tg-c3ow">1008</td>
    <td class="tg-c3ow">4976</td>
    <td class="tg-c3ow">2282</td>
    <td class="tg-c3ow">2416</td>
    <td class="tg-c3ow">3937</td>
    <td class="tg-c3ow">89.70</td>
  </tr>
  <tr>
    <td class="tg-c3ow" rowspan="3">III</td>
    <td class="tg-c3ow">|N<sub>C</sub>|</td>
    <td class="tg-c3ow">1162</td>
    <td class="tg-c3ow">9809</td>
    <td class="tg-c3ow">4042</td>
    <td class="tg-c3ow">5067</td>
    <td class="tg-c3ow">8758</td>
    <td class="tg-c3ow">n/a</td>
  </tr>
  <tr>
    <td class="tg-c3ow">|N<sub>R</sub>|</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-c3ow">158</td>
    <td class="tg-c3ow">4</td>
    <td class="tg-c3ow">23</td>
    <td class="tg-c3ow">158</td>
    <td class="tg-c3ow">n/a</td>
  </tr>
  <tr>
    <td class="tg-c3ow">|Onto|</td>
    <td class="tg-c3ow">5112</td>
    <td class="tg-c3ow">9783</td>
    <td class="tg-c3ow">7277</td>
    <td class="tg-c3ow">7195</td>
    <td class="tg-c3ow">9179</td>
    <td class="tg-c3ow">94.45</td>
  </tr>
  <tr>
    <td class="tg-7btt" colspan="2">BioPortal</td>
    <td class="tg-7btt">Min</td>
    <td class="tg-7btt">Max</td>
    <td class="tg-7btt">Med</td>
    <td class="tg-7btt">Mean</td>
    <td class="tg-7btt">90Ptl</td>
    <td class="tg-7btt">%</td>
  </tr>
  <tr>
    <td class="tg-c3ow" rowspan="3">I</td>
    <td class="tg-c3ow">|N<sub>C</sub>|</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-c3ow">784</td>
    <td class="tg-c3ow">127</td>
    <td class="tg-c3ow">192</td>
    <td class="tg-c3ow">214</td>
    <td class="tg-c3ow">n/a</td>
  </tr>
  <tr>
    <td class="tg-c3ow">|N<sub>R</sub>|</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-c3ow">122</td>
    <td class="tg-c3ow">5</td>
    <td class="tg-c3ow">15</td>
    <td class="tg-c3ow">17</td>
    <td class="tg-c3ow">n/a</td>
  </tr>
  <tr>
    <td class="tg-c3ow">|Onto|</td>
    <td class="tg-c3ow">10</td>
    <td class="tg-c3ow">794</td>
    <td class="tg-c3ow">283</td>
    <td class="tg-c3ow">312</td>
    <td class="tg-c3ow">346</td>
    <td class="tg-c3ow">96.89</td>
  </tr>
  <tr>
    <td class="tg-c3ow" rowspan="3">II</td>
    <td class="tg-c3ow">|N<sub>C</sub>|</td>
    <td class="tg-c3ow">5</td>
    <td class="tg-c3ow">4530</td>
    <td class="tg-c3ow">1185</td>
    <td class="tg-c3ow">1459</td>
    <td class="tg-c3ow">1591</td>
    <td class="tg-c3ow">n/a</td>
  </tr>
  <tr>
    <td class="tg-c3ow">|N<sub>R</sub>|</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-c3ow">131</td>
    <td class="tg-c3ow">12</td>
    <td class="tg-c3ow">30</td>
    <td class="tg-c3ow">33</td>
    <td class="tg-c3ow">n/a</td>
  </tr>
  <tr>
    <td class="tg-c3ow">|Onto|</td>
    <td class="tg-c3ow">1023</td>
    <td class="tg-c3ow">4977</td>
    <td class="tg-c3ow">2401</td>
    <td class="tg-c3ow">2619</td>
    <td class="tg-c3ow">2782</td>
    <td class="tg-c3ow">97.18</td>
  </tr>
  <tr>
    <td class="tg-c3ow" rowspan="3">III</td>
    <td class="tg-c3ow">|N<sub>C</sub>|</td>
    <td class="tg-c3ow">432</td>
    <td class="tg-c3ow">8340</td>
    <td class="tg-c3ow">4363</td>
    <td class="tg-c3ow">4387</td>
    <td class="tg-c3ow">4806</td>
    <td class="tg-c3ow">n/a</td>
  </tr>
  <tr>
    <td class="tg-c3ow">|N<sub>R</sub>|</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-c3ow">135</td>
    <td class="tg-c3ow">17</td>
    <td class="tg-c3ow">30</td>
    <td class="tg-c3ow">34</td>
    <td class="tg-c3ow">n/a</td>
  </tr>
  <tr>
    <td class="tg-c3ow">|Onto|</td>
    <td class="tg-c3ow">5084</td>
    <td class="tg-c3ow">8836</td>
    <td class="tg-c3ow">6934</td>
    <td class="tg-c3ow">6912</td>
    <td class="tg-c3ow">7109</td>
    <td class="tg-c3ow">98.72</td>
  </tr>
</tbody>
</table>
</div>

## Import of this project

* Unzip this project.
* Import it into IDEA.
* Make the src folder as source root.
* Make sure that the jar package under the root folder has been added into project as libriaries.

## Description of the UI tool

* The UI tool is a high-performance prototype for computing uniform interpolants of **ALCI-Ontologies**. It can be used as a Java library or a standalone tool for UI and related tasks.

* A uniform interpolant provides a restricted view of an ontology using only a subset of its signature (the interpolation signature) while preserving all logical entailments over this subset in the absence of other names from the original signature. It can be computed by incrementally forgetting names outside the interpolation signature—collectively forming the complementary forgetting signature—while maintaining all logical entailments expressible in the interpolation signature.

* If an input ontology is not an ALCI one, our tool simply takes the ALCI fragment of the ontology and discards those axioms not expressible in ALCI. If an input ontology contains cyclic dependencies over the names in the forgetting signature, the result cannot always be represented finitely without fixpoint operators. Since fixpoint operators are not supported by OWL API, our UI tool introduces additional concept names, namely definers, to the output ontology that simulate the behaviour of fixpoint operators. In this sense, the result is no longer a uniform interpolant, since it contains extra names that are not in the specified interpolation signature.

## Run of the UI tool

* To run the forgetting method, go to  **/src/forgetting/Forgetter.class** and call the method: 

  ```java
  public Set<OWLAxiom> ForgettingAPI(Set<OWLObjectProperty> roles, Set<OWLClass> concepts, OWLOntology onto)
  ```

* The input are a set of role names to be forgotten  ( ``` Set<OWLObjectProperty> roles ``` ),  a set of concept names to be forgotten ( ``` Set<OWLClass> concepts ``` ) and an ALCI-Ontologies from which the concept and role names are forgotten ( ``` OWLOntology onto ``` ).

* The output is another ALCI-Ontology which is a uniform Σ-interpolant of the ontology ``onto``, represented as a set of OWLAxioms.

* An example illustrating the usage of the UI tool is included in the Forgetter.class main function.
