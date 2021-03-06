
'vtreat' 0.5.31 2017/01/23

Changes:

- make prueSig an optional argument in prepare, and force by-name access.
- Remove left.op=TRUE from findInterval in "vtreat Rare Levels" vignette (seems to be a new addition to findInterval, so fails CRAN check r-oldrel-windows-ix86+x86_64).


'vtreat' 0.5.30 2017/01/21

Changes:

- General improvements in documentation and vignettes.
- Document saving/loading treatment plans.


'vtreat' 0.5.29 2016/10/27

Changes:

- Add 'rsq' column to scoreFrame (rsq- for numeric targets, pseudo-rsq for categorical targets).

'vtreat' 0.5.28 2016/10/24

Changes:

- Fix treatment of constant columns in cross-partitions.
- Switch doCollar default to FALSE.
- Return indicators on designTreatmentsZ.
- Fix extraDegreesOfFreedom calculation.
- Allow repeated application rows in cross frames.
- Remove lsig and csig from scoreFrame.
- Add meanY to treatmentplan.
- Documentation fixes.


'vtreat' 0.5.27 2016/08/16

Changes:

- Change catB variables to delta-logit score.
- Fix passing of arguments to parallel prepare, and reduce size of data passed.
- Ensure set of variables consistency in mkCross* methods.
- More parallelization of level significance calculations, and cheaper chi-square test where appropriate.

'vtreat' 0.5.26 2016/07/10

Changes:

- Facilities for y-stratified and grouped splitting (useful for unbalanced classes).
- catScaling=TRUE mode uses logistic regression for y-aware variable scaling.
- Fix erroneous bad type warning on date columns.


'vtreat' 0.5.25 2016/05/02

Changes:

- Fix bug that caused catB variables to be scored as "insignificant".
- Add test to check for above bug.
- Expose cross validation controls.
- More guards on significance calculations.


'vtreat' 0.5.23 2016/04/28

Changes:

- Fix issue of non-significant variables not being scaled.
- Documentation fixes, document variable types, improve vignettes.
- Minor performance fixes on result accumulation.
- Add optional use of dplyr for row binding (of score report frames).


'vtreat' 0.5.22 2016/01/07

Changes:

- Calculations of non catX significances are now deterministic
- Catch mis-naming or non-varying y earlier
- Expose buildEvalSets as a public function
- More tests


'vtreat' 0.5.21 2015/11/23

Changes:

- Isolated "cross" or "out of sample" frame generation into mkCrossFrameCExperiment() and mkCrossFrameNExperiment()
- Many small bug fixes and corner cases patched


'vtreat' 0.5.20 2015/11/05

Changes:

- Simplified out of sample frame generation
- Added "no-Y" treatment option
- Minor documentation fixes


'vtreat' 0.5.18 2015/10/07

Changes:

- Fixed bugs in cross-validated mode
- Force out of sample calculations in more situations
- Fix vignette titles
- Fix documentation
- Do not allow small or insufficiently varying data frames (exact conditions in documentation)


'vtreat' 0.5.16 2015/09/12

Changes:

-  Unified rare level treatment
-  Separate treatment of insignificant levels
-  Tests confirming compatibility with 'data.table'
-  More special case hardening
-  Over-fit vignette
-  Minor documentation fixes



'vtreat' 0.5.14 2015/09/06

- First CRAN release
