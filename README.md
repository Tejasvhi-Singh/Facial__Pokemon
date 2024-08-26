## Initial Setup and Data Extraction

### Overview:
On Day 1, the primary focus was on setting up the environment, fetching Pokémon data from Bulbapedia, and preparing for image extraction. The goal was to automate the process of collecting Pokémon names, their forms, types, and associated images from the Bulbapedia website.

### Tasks Completed:
1. **Environment Setup:**
   - Initialized a Python environment for web scraping and data processing tasks.
   - Installed and imported necessary libraries including `requests` and `BeautifulSoup` for handling HTTP requests and parsing HTML content.

2. **Data Extraction:**
   - Fetched the Pokémon list from the [Bulbapedia National Pokédex page](https://bulbapedia.bulbagarden.net/wiki/List_of_Pok%C3%A9mon_by_National_Pok%C3%A9dex_number).
   - Parsed the HTML content to extract Pokémon names, forms (e.g., Galarian, Alolan), and types.
   - Addressed special cases like Mr. Mime, which required careful handling due to its unique name structure.

3. **Data Structuring:**
   - Structured the extracted data into a CSV format, including columns for Pokémon index, name, and types.
   - Ensured the correct handling of Pokémon with multiple forms by appending the form name (e.g., _Galarian) to the title.

4. **Image Download Preparation:**
   - Parsed the image URLs associated with each Pokémon and prepared the filenames for downloading.
   - Developed a script to automatically download and save images using the Pokémon index and name, ensuring accurate naming for different forms.

5. **Image Download Script:**
   - Implemented a Python script to download Pokémon images from the Bulbapedia website.
   - Saved the images with filenames in the format `#_Name_Form.png` (e.g., `1_Bulbasaur.png`, `19_Rattata_Alolan.png`).

### Summary:
The first phase of the project laid the groundwork for automating the extraction and storage of Pokémon data. By the end of Day 1, a robust pipeline was in place for fetching and structuring data, handling special cases, and downloading related images with accurate naming conventions.

### Next Steps:
- Review the extracted data and downloaded images for accuracy.
- Optimize the scripts for efficiency and scalability.
- Prepare for further analysis and data manipulation in the upcoming phases.
