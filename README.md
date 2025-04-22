# Mongo-DB-project

🗂️ Project Overview

This project explores the implementation of a batch processing system using the Spotify Web API and MongoDB, a NoSQL JSON document database. The primary objective is to demonstrate how structured and semi-structured data can be ingested, stored, and queried at scale using MongoDB in the context of digital music streaming data. By simulating a real-world analytics pipeline, the project emphasizes the use of modern data engineering tools to support music trend analysis and user preference modeling.

The system addresses a key problem in music recommendation and data-driven insights: “How can large volumes of music metadata be collected, processed, and analyzed efficiently?”

🎯 Key Objectives

The main goal of the project was to develop a batch processing solution that retrieves large volumes of music-related data via the Spotify API and stores them in MongoDB collections for structured querying. The project emphasizes integrating cloud-based database solutions with external APIs and performing various analytical queries on the collected data to extract meaningful insights related to tracks, artists, and genres. It also highlights the practical use of JSON document storage for flexible and scalable data management.

📊 Data Collection & Features

Data was obtained using the Spotify API by querying endpoints for artists, albums, and tracks. The batch collection focused on compiling complete metadata for top songs and albums across multiple genres and regions. The project employed authenticated requests through Spotify’s SDK and applied filtering mechanisms to retrieve high-quality records.

The dataset included features such as track names, artist details, popularity scores, release dates, duration, genres, and unique Spotify URIs.

Key challenges in this stage included managing API rate limitations, transforming nested JSON responses into flattened structures suitable for MongoDB insertion, and maintaining data consistency across multiple requests.

🧠 Data Storage & Querying with MongoDB

A free cloud cluster was created using MongoDB Atlas. Spotify data was stored in collections representing entities such as artists, tracks, and albums. The project demonstrated how to perform CRUD (Create, Read, Update, Delete) operations using PyMongo, MongoDB’s official Python driver.

The collected data was inserted into MongoDB as nested JSON documents, preserving their flexible schema structure. Aggregation pipelines were used to perform queries for analytics, including filtering top artists by popularity, grouping tracks by genre and release year, and evaluating the distribution of track durations.

Efficient indexing strategies and document modeling were implemented to ensure performant querying for analytical purposes.

📈 Visualization Highlights

While the core of this project focused on backend database operations, summary-level insights were visualized using tables and textual output generated from MongoDB queries. These outputs included lists of the most-streamed artists, genres with the highest average popularity, and distributions of track release years across the dataset.

This data was essential for validating the success of the batch processing pipeline and the usefulness of MongoDB for large-scale music data analytics.

⚙️ Tech Stack

This project was built using the following technologies:

Python

Spotify Web API for data extraction

MongoDB Atlas for cloud-hosted NoSQL data storage

PyMongo for MongoDB interactions

Google Colab as the development environment

💡 Key Insights

The analysis revealed that certain genres like pop and hip-hop consistently ranked highest in artist and track popularity. Moreover, most popular songs were found to be concentrated in recent release years, reflecting trends in streaming consumption. The use of MongoDB’s flexible schema design enabled seamless ingestion of deeply nested Spotify JSON data, which would have posed challenges in traditional relational databases.

🔮 Future Enhancements

Potential future improvements include expanding the dataset to cover regional charts, integrating audio features such as tempo and acousticness for deeper song analysis, and deploying a web dashboard to visualize trends interactively. Additionally, incorporating time-based querying and real-time updates would further align the system with industry-grade data streaming and analytics pipelines.

📞 Contact

Harjoban Singh 

📧 hjawanda@norquest.ca

📞 +1 (780)-224-0890
