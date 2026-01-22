# Market Basket Analysis using FP-Growth

## Project Title
Market Basket Analysis using FP-Growth Algorithm

## File
MARKET-BASKET-ANALYSIS-USING-FPGROWTH.ipynb

## Objective
The objective of this project is to discover frequent itemsets and generate meaningful association rules from transactional data using the FP-Growth (Frequent Pattern Growth) algorithm. This helps uncover hidden purchasing patterns and relationships between products.

## Description
Market Basket Analysis is widely used in retail and e-commerce to understand customer buying behavior. In this project, the FP-Growth algorithm is applied to transactional data to efficiently mine frequent itemsets without candidate generation. Compared to Apriori, FP-Growth significantly reduces computational cost by using a compact data structure called the FP-tree.

The notebook preprocesses transaction data, builds the FP-tree, extracts frequent itemsets, and generates association rules based on support, confidence, and lift.

## Dataset
- Type: Transactional dataset
- Format: Each row represents a transaction containing multiple items
- Example use case: Grocery store purchase history
- Source: Local CSV file (or user-provided dataset)

## Algorithm Used
FP-Growth (Frequent Pattern Growth)

Key characteristics:
- Uses FP-tree data structure
- Avoids candidate generation
- Efficient for large and sparse datasets
- Faster than Apriori in most real-world cases

## Steps Involved
1. Import required libraries
2. Load and clean the dataset
3. Convert transactions into one-hot encoded format
4. Apply FP-Growth algorithm
5. Set minimum support threshold
6. Generate frequent itemsets
7. Generate association rules using confidence and lift
8. Display and analyze results

## Libraries Used
- pandas
- mlxtend.frequent_patterns
- mlxtend.preprocessing

## Output
- Frequent itemsets with support values
- Association rules with:
  - Support
  - Confidence
  - Lift

## Use Cases
- Product recommendation systems
- Cross-selling and up-selling strategies
- Store layout optimization
- Inventory planning
- Customer behavior analytics

## Advantages of FP-Growth
- No candidate generation
- High performance on large datasets
- Scales well with number of transactions
- Produces both itemsets and association rules

## Limitations
- FP-tree can consume memory for extremely large datasets
- Requires preprocessing into transactional/encoded format
- Interpretation of large rule sets can be complex

## How to Run
1. Open the notebook MARKET-BASKET-ANALYSIS-USING-FPGROWTH.ipynb
2. Verify dataset file path
3. Install required libraries (mlxtend if missing)
4. Run all notebook cells sequentially
5. Review generated itemsets and association rules

## Conclusion
This project demonstrates the effectiveness of the FP-Growth algorithm for market basket analysis. By efficiently mining frequent itemsets and association rules, it provides actionable insights into customer purchasing behavior, enabling better business and marketing decisions.

## Author
Developed as part of a data mining / machine learning practical implementation.
