# SafeCab — Women’s Safety Ride-Share Estimator

SafeCab is a smart routing system designed to help women choose the __safest and most cost-effective ride-share routes__. It analyzes crime data, lighting conditions, fare, and distance to recommend the **safest + cheapest** path and predicts if a route is "unsafe" using a machine learning classifier.

## Motivation

While existing ride-sharing apps prioritize cost and speed, __they often ignore safety__ which is a major concern for women traveling alone, especially at night. SafeCab aims to bridge this gap using data-driven safety routing.

## Features

-  Route scoring based on __crime rate, lighting, fare, and distance__
-  Computes the __safest + cheapest__ route using graph algorithms
-  Machine Learning classifier predicts whether a route is unsafe
-  Customizable weights (e.g., prioritize safety over fare)
-  Interactive frontend with live map display

## Tech Stack

- __Frontend__: React.js, Leaflet.js / Mapbox
- __Backend__: Node.js, Express.js
- __ML Model__: Python (Sklearn), FastAPI
- __Graph Search__: Dijkstra’s algorithm (with custom risk-weighted edges)
- __Data Sources__: OpenStreetMap, city crime datasets, lighting data, fare estimates

## Project Structure
SafeCab/
├── client/ # React frontend
├── server/ # Express backend for routing and API
├── ml-model/ # Python ML model to classify unsafe routes
├── graph/ # Graph algorithms (Dijkstra, scoring logic)
├── data/ # Crime, lighting, and road network data
└── README.md

