## Data Model Description

The dataset represents transactional sales records.

Each row corresponds to a single order line.

### Main Fields
- Order ID : Unique identifier for each order
- Order Date : Date of purchase
- Region : Geographic sales region
- Category : Product category
- Sub-Category : Product sub-type
- Sales Amount : Revenue generated
- Profit : Net profit from the sale
- Quantity : Units sold

### Relationships
The data was structured into a single fact table and analyzed using calculated measures.

Date hierarchy was used to analyze:
- Monthly trends
- Quarterly patterns
- Yearly performance

Data cleaning steps:
- Removed null values
- Standardized category names
- Converted date column to proper date format
