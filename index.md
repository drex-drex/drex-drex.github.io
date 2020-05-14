## Drex

Uncaught runtime exceptions have been recognized as one of the commonest root causes of real-world~exception bugs in Java applications. However, existing runtime exception detection techniques rely on symbolic~execution or random testing, which may suffer the scalability or coverage problem, while rule-based~bug~detectors (e.g., SpotBugs) provide limited rule support for runtime exceptions. Inspired by the recent successes~in~applying deep learning to bug detection, we propose a deep learning-based technique, named \tool, to identify~not~only the types of runtime exceptions that a method might signal but also the statement scopes that might signal the detected runtime exceptions. It is realized by graph-based code representation learning~with~(i)~a~lightweight analysis to construct a joint graph of CFG, DFG and AST for each method without requiring a build~environment so~as~to~comprehensively characterize statement syntax and semantics and (ii) an attention-based~graph~neural network to learn statement embeddings in order to distinguish different types of potentially signaled runtime exceptions with explainability. Our extensive evaluation on \todo{54,255}~methods~with~caught~runtime~exceptions~and \todo{54,255}~methods without caught runtime exceptions from \todo{5,996} GitHub Java projects~has~indicated~that~\tool improves baseline approaches by up to \todo{16.9\%} in exact accuracy and \todo{17.3\%} in F1-score. Our manual analysis~on \todo{40} methods has indicated that our lightweight analysis constructs CFG and DFG with~high~accuracy. \tool detects \todo{20} new uncaught~runtime~exceptions in \todo{13} real-world projects, \todo{7} of them have been confirmed and fixed, while none of them is detected by rule-based bug detectors (i.e., SpotBugs~and~PMD).The paper about this work has been submitted to oopsla 2020.



### Source Code

You can download the source code of Drex [here](code.zip)

### Dataset

Due to the large volume of our dataset, please contact *17839227248@163.com* for further use.
