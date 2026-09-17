## Data Cleaning & Validation

To ensure high data quality and accuracy across all visual reports, the raw dataset underwent a thorough cleaning and validation workflow in Google Sheets/Excel before analysis.

### Cleaning Steps Applied
* **Duplicate Removal:** Identified and eliminated duplicate entries based on unique order identifiers to prevent inflated transaction metrics.
* **Missing Value Treatment:** Imputed missing values across categorical attributes (e.g., `PaymentMethod`, `OrderStatus`) and assigned default values for missing promotional codes.
* **Format Standardization:**
  * Standardized all transaction dates to `YYYY-MM-DD`.
  * Converted numerical pricing and revenue fields into standard currency (`$ USD`).
  * Unified text casing across product names, referral sources, and order statuses to prevent grouping splits during pivot table aggregations.

### Data Validation Rules
* **Restricted Dropdowns:** Implemented Data Validation rules on key fields (`OrderStatus`, `PaymentMethod`) to ensure only approved status options can be entered.
* **Numeric & Date Range Checks:** Ensured order quantities, unit prices, and transaction dates fell within valid operational boundaries.
* **Calculated Field Verification:** Validated formula logic for gross revenue (`Quantity` × `UnitPrice`) across all rows to verify zero calculation errors.
