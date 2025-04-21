<a name="readme-top"></a>

<!--
!!! IMPORTANT !!!
This README is an example of how you could professionally present your codebase. 
Writing documentation is a crucial part of your work as a professional software developer and cannot be ignored. 

You should modify this file to match your project and remove sections that don't apply.

REQUIRED SECTIONS:
- Table of Contents
- About the Project
  - Built With
  - Live Demo
- Getting Started
- Authors
- Future Features
- Contributing
- Show your support
- Acknowledgements
- License

OPTIONAL SECTIONS:
- FAQ

After you're finished please remove all the comments and instructions!

For more information on the importance of a professional README for your repositories: https://github.com/microverseinc/curriculum-transversal-skills/blob/main/documentation/articles/readme_best_practices.md
-->

<div align="center">

</div>

<!-- TABLE OF CONTENTS -->

# 📗 Table of Contents

- [📖 Inferring Mobility from Mobile Phone Data](#about-project)
    - Togo Mobility Analytics is a Python project that processes mobile phone call detail records to estimate where subscribers live and how they move over time. Through data cleaning, visualization, and two complementary inference algorithms, it computes summary statistics, maps cell-tower distributions, and determines each user’s most likely home prefecture. Finally, it compares algorithmic agreement and tracks weekly location changes, offering insights for humanitarian and development planning while addressing privacy and ethical considerations.
  - [🛠 PYTHON](#built-with)
    - [Python 3.x
    - Jupyter Notebook for interactive analysis
    - `pandas` for data manipulation
    - `numpy` for numerical operations
    - `matplotlib` and seaborn for data visualization
    - `geopandas` and folium (or similar) for mapping towers (if implemented)
    - `scikit-learn` for clustering analysis]
  - [Key Features](#key-features)
     - Summary Statistics: Compute total transactions, unique callers/receivers, days covered, and average calls per subscriber.
     - Tower Mapping: Visualize cell tower locations over Togo's prefectural map and analyze spatial concentration.
     - Home Inference Algorithms:
     - Modal Nighttime Location: Identify home prefecture based on most frequent nighttime activity (8 PM–6 AM).
     - Mode of Modes: Determine daily modal location (day vs. night) and compute overall mode across days.
     - Algorithm Comparison: Quantify agreement and disagreement counts between inferred home locations.
     - Mobility Inference: Track weekly inferred locations for selected subscribers and measure missing data rates.
     - Ethical Reflection: Discuss applications in disaster response, poverty prediction, and public health, alongside privacy and bias concerns.
- [💻 Getting Started](#getting-started)
    - To get a local copy up and running, follow these steps.
  - [Prerequisites](#prerequisites)
    - Python 3.x
    - Jupyter Notebook or JupyterLab
    - Git for cloning the repository
  - [Setup](#setup)
     - Clone this repository: `git clone https://github.com/Marlyn-Mayienga/Inferring-Mobility-from-Mobile-Phone-Data.git`
  - [Install](#install)
     - Install dependencies: `pip install pandas numpy matplotlib seaborn geopandas folium scikit-learn`
  - [Usage](#usage)
     - Ensure the dataset files (`cdr.csv`, `tower_locations.csv`, `winequality-red.csv`) are in the project directory or the configured data/ folder.
     - Open the Jupyter Notebook `Assignment1.ipynb` in Jupyter.
     - Run all cells to reproduce the analysis:
     - Summary statistics (Part 1)
     - Tower mapping (Part 2)
     - Home inference algorithms and comparison (Part 3)
     - Weekly mobility inference (Part 4)
- [👥 Authors](#authors)
   - 👤 **Marlyn Mayienga**

- GitHub: [@Marlyn_Mayienga](https://github.com/Marlyn_Mayienga)
- Twitter: [@Merl_Mayienga](https://twitter.com/M_ayienga)
- LinkedIn: [Marlyn_Mayienga](https://linkedin.com/in/Marlyn_Mayienga)
- [🔭 Future Features](#future-features)
    - Add a third inference algorithm (e.g., random forest classification) for home location.
    - Build an interactive dashboard with real-time data updates.
    - Extend analysis to multi-country CDR datasets for comparative studies.
    - Integrate mobile app interface for visualizing individual subscriber paths.

- [🤝 Contributing](#contributing)
    - Fork the project
    - Create your feature branch (`git checkout -b feature/AmazingFeature`)
    - Commit your changes (`git commit -m 'Add some AmazingFeature'`)
    - Push to the branch (`git push origin feature/AmazingFeature`)
    - Open a pull request
- [⭐️ Show your support](#support)
   - If you like this project, please give it a ⭐️ on GitHub!
- [🙏 Acknowledgements](#acknowledgements)
   - R. Warren, E. Aiken, and J. Blumenstock, “Home Location Detection from Mobile Phone Data: Evidence from Togo,” COMPASS ’22.
   - “Machine learning and phone data can improve targeting of humanitarian aid,” Nature.
   - J. Blumenstock et al., “Predicting poverty and wealth from mobile phone metadata,” Science, 2015.
   - “Using Mobile Phone Data to Predict the Spatial Spread of Cholera,” Scientific Reports.
- [❓ FAQ (OPTIONAL)](#faq)
- [📝 License](#license)
   - This project is [MIT](./LICENSE) licensed.

_NOTE: we recommend using the [MIT license](https://choosealicense.com/licenses/mit/) - you can set it up quickly by [using templates available on GitHub](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository). You can also use [any other license](https://choosealicense.com/licenses/) if you wish._

<p align="right">(<a href="#readme-top">back to top</a>)</p>
