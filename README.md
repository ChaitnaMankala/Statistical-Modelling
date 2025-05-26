# Statistical Modelling
This project explores the relationship between various musical features and the popularity of music tracks using statistical modelling techniques in Python. It demonstrates the end-to-end process of data cleaning, exploratory data analysis, visualization, and linear regression modelling to uncover key insights into what makes a track popular.

**Objective**
The goal is to use statistical modelling to:
- Analyze how features like danceability, energy, loudness, acousticness, and valence influence the popularity of songs.
- Identify the features that are statistically significant in determining a track's popularity.
- Compare trends across explicit and non-explicit tracks.

**Dataset**
The dataset includes 100 music tracks and their metadata such as:
- Track Name, Artist, Album
- Popularity score
- Musical features (Danceability, Energy, Loudness, Valence, Tempo, etc.)
- Explicit content flag

**Tools & Libraries**
- Pandas for data handling
- Matplotlib & Seaborn for data visualization
- Scikit-learn for preprocessing and linear regression modelling
- NumPy for numerical operations

**Project Workflow**
1. Data Preprocessing
   - Removed unnecessary columns (Unnamed: 0)
   - Handled missing values in textual fields (filled with 'Unknown')
   - Converted boolean Explicit to integer format for modelling
2. Exploratory Data Analysis
   - Visualized popularity distribution
   - Generated correlation heatmap
   - Created scatter plots of individual features vs popularity
3. Feature Analysis by Explicit Content
   - Compared the trends of explicit vs non-explicit tracks in terms of danceability and energy
4. Statistical Modelling (Linear Regression)
   - Standardized numeric features
   - Built a linear regression model
   - Evaluated model using Mean Squared Error and R² Score
   - Analyzed model coefficients to interpret feature importance

**Key Insights**
- Positive influencers: Danceability, Loudness, Acousticness, and Valence show a strong positive relationship with popularity.
- Negative influencers: Higher Energy, Key, Mode, and Tempo tend to negatively impact popularity.
- Negligible effects: Explicit content and Speechiness showed minimal influence.
