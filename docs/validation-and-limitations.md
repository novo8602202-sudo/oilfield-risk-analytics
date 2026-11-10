# Validation, disclosure and limitations

## Evidence levels

**Confirmed in the supplied research artifacts:** Python/Jupyter workflow for data profiling, factor analysis, candidate threshold estimation, comparisons of several machine-learning algorithms, interpretability rules, and Excel export.

**Described in accompanying technical reports:** application to historical well workovers, reviewed pilot cases, estimated schedule/cost differences, and agreement with selected past engineering decisions.

**Not independently confirmed by a public reproducible dataset:** external predictive accuracy, financial savings realized after deployment, reliability on future wells, and generalization across fields.

## Known modeling cautions

- The available sample is relatively small for robust multivariate modeling.
- Model comparison and threshold selection may be sensitive to sampling and data leakage; evaluation should be nested where needed.
- Regression of workover duration had weak cross-validation evidence in the inspected stage.
- The threshold rule is an interpretable heuristic requiring ongoing validation.
- Operational recommendations are contingent on the engineering context.

## Disclosure policy

Do not publish:
- Identifiable wells, pads, field-specific raw measurements or internal work orders
- Original company datasets or source notebooks that contain confidential details
- Detailed production economics, raw presentations or names of individual personnel
- Credentials, API keys, internal addresses, or private contact information

Use descriptions, aggregate methodology and synthetic illustrative examples only.
