Movie Recommendation System (MRS)
A simple, command-line movie recommendation system that suggests similar movies using a content-based filtering model. Enter your favorite movie, and get a list of similar ones to watch next!

Features
Content-Based Recommendations: Suggests movies based on similarity in their metadata (genre, keywords, overview, etc.).

Simple CLI: An easy-to-use command-line interface to get instant recommendations.

Customizable: You can easily modify the dataset and retrain the model to customize the recommendations.

Cosine Similarity Model: Utilizes a robust and popular method for measuring content similarity.

Installation Guide
Follow these steps to set up and run the project on your local machine.

1. Prerequisites
Make sure you have Python 3.8 or a newer version installed. You can check your Python version with:

Bash

python --version
2. Clone the Repository
First, clone this repository to your local machine.

Bash

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
(Note: Replace the URL with the actual link to your repository.)

3. Create a Virtual Environment
It is a best practice to create a virtual environment to manage project dependencies without affecting your global Python installation.

Bash

# For Windows
python -m venv venv
.\venv\Scripts\activate

# For macOS / Linux
python3 -m venv venv
source venv/bin/activate
4. Install Dependencies
With your virtual environment activated, install all the required packages using the requirements.txt file.

Bash

pip install -r requirements.txt
How to Run
Once the installation is complete, you can run the recommendation system from the project's root directory.

Execute the main script in your terminal:

Bash

python main.py
When prompted, enter the full name of a movie you like and press Enter.

Example Usage
Here is an example of how the command-line interface works:

Enter a movie you like: The Dark Knight
-----------------------------------------
Recommendations for "The Dark Knight":
1. The Dark Knight Rises
2. Batman Begins
3. Batman
4. Batman Returns
5. Inception
-----------------------------------------
Note: This is a script-based application and does not include a web or graphical user interface (GUI).

Model Details
This system uses a content-based filtering approach, which recommends items based on their attributes.

Core Technique: The model calculates the cosine similarity between the feature vectors of movies. A higher cosine similarity score between two movies means they are more alike in terms of content.

Feature Extraction: For each movie in the movies.csv dataset, a combined feature string is created from its metadata (e.g., genres, keywords, director, main cast, overview). This text is then converted into a numerical vector using a TF-IDF Vectorizer.

Recommendation Logic: When you input a movie, the system finds its pre-calculated vector and compares it against the vectors of all other movies. The movies with the highest similarity scores are then presented as the top recommendations.

Dataset: The initial model is trained on movies.csv, which contains data for approximately the top 2500 movies.

About the Developer
Name: Arpan Patel

University: Galgotias University

Course: B.Tech CSE – 2025

This project was built for learning and demonstration purposes.
