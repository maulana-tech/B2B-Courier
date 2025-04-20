# B2B Courier Analysis

## Project Overview
This project analyzes courier service charges and billing discrepancies for a B2B (Business-to-Business) courier operation. The analysis helps identify overcharging and undercharging instances by comparing expected charges with actual billed amounts.

## Data Sources
The project uses the following data files:
- `Order Report.csv` - Contains order details and SKU information
- `SKU Master.csv` - Contains product SKU and weight information
- `pincodes.csv` - Maps warehouse and customer pincodes to delivery zones
- `Courier Company - Rates.csv` - Contains courier company rate cards for different zones
- `Invoice.csv` - Contains actual billing information from the courier company

## Analysis Components
1. **Data Preprocessing**
   - Removal of unnecessary columns
   - Merging of relevant datasets
   - Weight conversion from grams to kilograms
   - Weight slab calculation

2. **Charge Calculation**
   - Expected charge calculation based on:
     - Delivery zones
     - Weight slabs
     - Shipment types (Forward/RTO)
   - Comparison with actual billed amounts

3. **Discrepancy Analysis**
   - Identification of correctly charged orders
   - Detection of overcharged orders
   - Detection of undercharged orders
   - Calculation of total discrepancy amounts

## Key Findings
The analysis revealed:
- 12 orders were correctly charged
- 382 orders were overcharged (Total overcharge: Rs. 33,750.5)
- 7 orders were undercharged (Total undercharge: Rs. -165.2)

## Visualization
The project includes a pie chart visualization showing the proportion of correctly charged, overcharged, and undercharged orders.

## Dependencies
- Python 3.x
- Pandas
- Plotly

## Usage
1. Ensure all data files are in the same directory as the notebook
2. Install required dependencies
3. Run the Jupyter notebook `B2B_Courier.ipynb`

## Author
Maulana

## License
This project is licensed under the MIT License - see the LICENSE file for details.