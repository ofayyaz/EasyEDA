1. Data Analysis Streamlit App

This Streamlit app is designed to facilitate the exploration and visualization of datasets with both categorical and numerical attributes. It provides functionalities such as file uploading, data viewing, statistical analysis, and interactive visualizations including heat maps, outlier detection, and histograms.

2. Features

- Upload CSV data files.
- Select attributes to analyze and visualize.
- View dataset statistics and customized plots.
- Explore correlations and outliers within the data.
- Interactive UI with sidebar controls.


3. How to Use the App

3.1. Expected Input

3.1.1. CSV Data Fil*: The application expects a CSV file to be uploaded by the user. This file should contain the dataset to be analyzed, with both categorical and numerical attributes.

3.1.2. User Selections: Through the Streamlit sidebar, the user can select:
   - A categorical attribute for analysis.
   - A numerical attribute for analysis.
   - A target attribute for heatmap and outlier analysis.
   - The type of dataframe to view (full, numerical, or categorical).

3.1.3. Toggle Switches and Options: Users can toggle views for different visualizations and select specific options for more detailed analysis.

3.2. Expected Output

3.2.1. Charts Tab (📈 Chart):
   - Displays a series of plots comparing the selected categorical attribute with various statistics of the selected numerical attribute (e.g., counts, median, mean, relative mean difference).

3.2.2. Data Tab (🗃 Data):
   - Shows the uploaded data in the selected format (full, numerical, or categorical).
   - Provides a detailed view of the number of attributes, number of records, and specific details for categorical attributes.

3.2.3. Heat Map Tab (🌡 Heat Map):
   - Renders a heatmap showing the correlation matrix for numerical attributes in the dataset. Users can toggle between a full heatmap and a heatmap showing only significant correlations.

3.2.4. Outliers Tab (🔢 Outliers):
   - Visualizes potential outliers in the data by comparing features against the target attribute. Outliers are highlighted for further investigation.

3.2.5. Histograms Tab (📊 Histograms):
   - Generates histograms for all numerical attributes in the dataset and provides summary statistics.

3.2.6. Statistical Summary:
   - Calculates and displays a statistical summary for the selected numerical attribute, including mean, median, and the relative difference between mean and median.

3.3. Example Usage Scenario

3.3.1. A user uploads a CSV file with sales data.
3.3.2. The user selects 'Region' as the categorical attribute and 'Sales' as the numerical attribute.
3.3.3. The app then calculates and visualizes the median and mean sales per region, along with the count of entries per region.
3.3.4. The user can explore correlations between sales and other numerical attributes in the dataset using the heatmap tab.
3.3.5. The outliers tab allows the user to identify regions where sales significantly deviate from the norm.

3.4. Installation

To use this app, you will need to have Python installed on your machine, along with the required libraries. To get started:

1. Clone this repository.
2. Create a virtual environment (optional).
3. Install the required dependencies.

```bash
git clone <repository-url>
cd <repository-name>
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt

Run the Streamlit app by navigating to the app's directory and executing the following command:
streamlit run app.py
