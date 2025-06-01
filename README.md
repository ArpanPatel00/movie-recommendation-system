
# Movie Recommendation System (MRS)

This repository contains all the project files and necessary details about how to run the project on your local machine.

| Title                                    | Description                                                 |
| ---------------------------------------- | ----------------------------------------------------------- |
| Requirements :heavy_check_mark:          | Requirements and essential links to get started             |
| Running in Local :desktop_computer:      | Instructions to run the project on your local machine       |
| Model Training :bar_chart:               | Basic idea behind how the model was prepared                |

<hr>

## Requirements :heavy_check_mark:

To build this project without any errors/issues, the following requirements need to be satisfied:

1. Python version >= 3.8 (Tested on 3.9.16)
2. Install the dependencies from the requirements.txt file:

```bash
pip install -r requirements.txt
```

<hr>

## Running in Local :desktop_computer:

Make sure your environment is activated and you're in the project root directory.

Run the following command:

```bash
python manage.py runserver

```

You can now use the command-line interface to search and get movie recommendations based on your input.

Note: This version is script-based and does not include any web interface.

<hr>

## Model Training :bar_chart:

This system uses a content-based filtering model trained using cosine similarity on movie metadata.

The model uses:
- Movie titles and descriptions
- Cosine similarity between feature vectors

You can modify the dataset (`movies.csv`) and retrain the model using the main script to improve or customize recommendations.

<hr>

## About

**Developed by:** Arpan Patel  
**University:** Galgotias University  
**Course:** B.Tech CSE – 2025

---

This project was built for learning and demonstration purposes. Only the top ~2500 movies (e.g., based on IMDb ratings) are included in the dataset.

---
