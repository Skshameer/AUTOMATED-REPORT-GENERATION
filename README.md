# AUTOMATED-REPORT-GENERATION
"COMPANY NAME": CODETECH IT SOLUTIONS

"NMAE" : SHAIK SHAMEER

"INTERN ID" : CT04DH281

"DOMAIN" : PYTHON

"DURATION" : 4 WEEKS

"MENTOR" : NEELA SANTHOSH

DESCRIPTION: Code-1: Creating CSV and Summary PDF Report The first part of the code creates a CSV file named data.csv and populates it with sample sales data. This data includes the date of sale, product name, units sold, and revenue. The csv module is used to write a list of lists to the file, ensuring the correct structure.

Next, the read_data() function reads this CSV using pandas, which converts the file into a DataFrame and returns a descriptive statistical summary using .describe(). This summary includes metrics like count, mean, standard deviation, minimum, and maximum for the numeric columns (Units Sold and Revenue).

The function generate_pdf_report() uses the reportlab library to create a PDF file titled report.pdf. It writes the summary statistics into the PDF in a tabular form. The statistics’ names (e.g., mean, std, min) and their corresponding values are written row-by-row. The layout is adjusted using coordinate positioning to ensure the content is spaced properly.

Code-2: Generating Detailed Sales PDF from CSV The second part of the code is designed to generate a detailed PDF report of the original dataset (data.csv) rather than a statistical summary. It again uses pandas to read the CSV into a DataFrame. The function generate_pdf_report() here creates a new PDF (sales_report.pdf) and formats it with headers for Date, Product, Units Sold, and Revenue.

Each row of the CSV data is iterated over using DataFrame.iterrows(), and the corresponding values are drawn onto the PDF using fixed x, y coordinates. The currency is formatted to show the revenue in rupees (₹) with two decimal points. Line spacing is handled manually by decrementing the y_position.

Conclusion These scripts together demonstrate a basic pipeline: data creation, analysis, and reporting. They are useful for automating business reporting tasks, converting raw data into human-readable formats. pandas handles data manipulation, while reportlab enables professional-quality PDF report generation. The approach can be scaled for larger datasets, integrated with real-time data sources, or enhanced with charts and styling. Image sales_report (1).pdf

<img width="827" height="115" alt="image" src="https://github.com/user-attachments/assets/9e77a1c6-23ca-4593-aa4a-9e0689ab98f8" />
