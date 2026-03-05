# 🎬 Movie Recommender System

### 🚩 Problem Statement
With the explosion of streaming content, "choice paralysis" has become a major user experience hurdle. Users need a system that understands the underlying themes and metadata of movies they enjoy to suggest relevant next-watches without relying purely on high-traffic popularity.

### 🧠 The Approach
I developed a **Content-Based Filtering** engine that focuses on the "DNA" of a movie:
1.  **Feature Engineering:** Combined movie metadata (genres, keywords, cast, and crew) into a single "tag" for each of the 5,000+ movies in the dataset.
2.  **Vectorization:** Implemented **TF-IDF (Term Frequency-Inverse Document Frequency)** to transform text tags into a numerical vector space, effectively penalizing common words and highlighting unique plot elements.
3.  **Similarity Modeling:** Calculated the **Cosine Similarity** between movie vectors. This allows the system to find the "closest" movies in a high-dimensional space.
4.  **Deployment:** Built an interactive web dashboard using **Streamlit** to allow users to search and receive top-5 recommendations instantly.



### 📊 Results
* **Performance:** Achieved sub-second latency for similarity matrix lookups across 5,000+ titles.
* **UX:** The Streamlit interface provided a 100% automated recommendation loop without requiring backend restarts.

### 👤 Author
**Mithul Krishna Suresh** *2nd Year B.Tech CSE, NIT Bhopal*
