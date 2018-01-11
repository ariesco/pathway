# Pathway FM, a Full Maude extension of Pathway logic

This project presents different extensions of Pathway logic using Full Maude:
* A top transformation (**all_top.maude**) for rules that allows users to use narrowing
with Pathway logic specifications.
* A soft set extension (**softset.maude**) that allows users to extend rules with sets
of pairs `[att = val]`, where `att` is an attribute identifier and `val` its value,
which can be `0` (the attribute does not appear in the current state),
`1` (the attribute appears in the current state), or
`*` (we do not have/provide information about the attribute in the current state). This
extension also provides predefined functions for evaluating fuzzy information, so the
attributes with value are considered differently.
* A fuzzy matching extension (**finst.maude**), which modifies the current module at
the metalevel so more general compounds are used in rules in order to enable them in
more contexts.

All extensions are loaded by the main file, **pathway_fm.maude**, and can be used once
this file is loaded.