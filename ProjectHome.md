Sireum is a long-term research effort to develop an over-arching software analysis platform that incorporates various static analysis techniques such as data-flow framework, model checking, symbolic execution, abstract interpretation, and deductive reasoning techniques (e.g., using weakest precondition calculation). It can be used to build various kinds of software static analyzers for different kinds of properties.

[Homepage](http://www.sireum.org)

# Sireum/Kiasan for Java #

Sireum/Kiasan for Java is a [JML](http://jmlspecs.org) contract-based automatic verification and test case generation tool-set for Java program units. In contrast to regular unit testing methods, Kiasan does not need input parameters for checking units. Without assertions or contracts (e.g., pre-/post-conditions), Kiasan, by default, detects possible uncaught runtime exceptions such as NullPointerException, ArithmeticException, ArrayIndexOutOfBoundsException, etc. With assertions embedded in the code, Kiasan automatically determines whether the assertions are possibly violated. When Java Modeling Language (JML) contracts (e.g., object/class invariants, method pre/postconditions) are supplied, Kiasan can leverage the contracts to ﬁlter out input parameters (i.e., pre-states) that do not satisfy the contracts while ensuring the states after execution (i.e., post-states) satisfy the contracts. In contrast to other bug ﬁnding tools, Kiasan generates a low number of false alarms due to its formal semantic-based analysis engine, and it has a stronger and quantiﬁable coverage on the unit behavior that it analyzes. Furthermore, Kiasan generates helpful analysis feedback by visualizing program states (e.g., object heap graphs) and JUnit test cases useful for illustrating property violations (e.g., assertion failures) as well as for code understanding or inspection (e.g., by visualizing code effects on program states).

## Documentation ##

  * [Manual](http://sireum.googlecode.com/files/sireum-kiasan-java-manual-v0.0.20081108.pdf)

## Sample Reports ##
  * [k <= 5](http://www.sireum.org/kiasan/report/k5)
  * [k <= 4](http://www.sireum.org/kiasan/report/k4)

## Downloads ##
  * [Sireum/Kiasan for Java](http://code.google.com/p/sireum/downloads/list) v0.0.20081108

> Platform: Java 5 or above

> Operating Systems: Mac OS X (32/64-bit), Linux (32/64-bit), and Windows (32-bit)

> Hardware: Intel x86 family

> Dependencies: [Yices](http://yices.csl.sri.com), [GraphViz](http://graphviz.org)