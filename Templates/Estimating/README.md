# Estimating Model Guidance

This model provides a quick way to estimate **Effort**, **Risk**, and **Cost** for initiatives using T-shirt sizing. It supports early-stage planning and decision-making where detailed estimates are not yet available.

## Purpose
- Enable rapid sizing for business cases, prioritization, and initial budgeting.
- Provide a consistent baseline for comparing initiatives.
- Supports both **overall sizing** and **attribute-level sizing**.

## Estimating Table

| Size | Effort (Work)   | Risk       | Cost   |
|------|-----------------|-----------|--------|
| S    | ≤ 4 weeks of effort | Low       | £50k   |
| M    | ≤ 2 months of effort| Moderate  | £100k  |
| L    | ≤ 3 months of effort| Significant| £150k |
| XL   | ≤ 4 months of effort| High      | £200k  |

> **Note:** Effort refers to the amount of work required (e.g., person-days), not elapsed calendar time.

### Scaling Beyond XL
If initiatives exceed XL:
- **Effort**: Add increments of **+1 month of effort** per size (e.g., XXL = 5 months, XXXL = 6 months).
- **Cost**: Add increments of **+£50k** per size (e.g., XXL = £250k, XXXL = £300k).
- **Risk**: Use descriptors like **Very High**, **Extreme**, or **Critical** for escalating uncertainty.

## How to Use

### **Option 1: Overall Size**
- Select **one size category (S, M, L, XL)** that best represents the initiative considering effort, risk, and cost together.
- Example: If cost is high but effort is low, you might choose **L** because financial impact outweighs delivery simplicity.

### **Option 2: Attribute-Level Sizing**
- Assign sizes individually for each dimension:
  - Effort: S  
  - Risk: XL  
  - Cost: M  
- Use this for nuanced discussions about trade-offs and complexity.

## Interpretation
- **Effort**: Approximate amount of work required (not elapsed time).
- **Risk**: Level of uncertainty and potential impact.
- **Cost**: Rough financial estimate.

## Flexibility
- Can be used for:
  - Business case development.
  - Input to 4MAT documents (“How Much” section).
  - Agile planning and backlog sizing.
- Adjust values for organizational norms or regional cost factors.

## Important Notes
- This is **not a substitute for detailed estimation**.
- Document assumptions when applying the model.
- Use for **early-stage decisions**, not final budgets.
