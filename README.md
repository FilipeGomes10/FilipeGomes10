Data Cleaning Project for HAW Hamburg Laboratory

This project was undertaken during my Erasmus semester at the Hochschule für Angewandte Wissenschaften Hamburg (HAW). The laboratory's filtering unit records data at short intervals, resulting in extensive datasets that make it difficult to distinguish between different experiments conducted on the same day.

To address this, I developed a Python function utilizing the pandas and numpy libraries. This function processes the raw data, identifies individual experiments, and splits them into separate Excel files, also summarizing the results for better readability.

Project Details

- User Input: The function begins by requesting the pressure value used in the experiments, which serves as the primary criterion for splitting the data.

- Data Cleaning: Unnecessary columns are removed from the initial Excel file to focus on relevant data.

- Averaging Data: The function calculates average values per minute for each column, reducing file size and improving clarity.

- Experiment Identification: By iterating through the pressure values, the function identifies the end of each experiment (when pressure drops below the provided value) and creates a new Excel file for each experiment.

- File Generation: This process repeats until all experiments are separated into individual files based on the pressure criteria.

This approach significantly enhances the manageability and analysis of the experimental data, providing clear and concise records for each experiment.

EXAMPLE CASE:

'data_cleaning_function' is the function; '0102.xlsx' is the input; the rest of the files are the outputs.
The experiments shown as a example were all made with a pressure of 12,5 bar.
