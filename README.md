# Traveling-Politician-Project

## Overview

This project implements a route optimization algorithm designed to calculate the most efficient route for a politician to travel to every U.S. state capital once, starting in Iowa and ending in Washington, DC. The objective is to minimize travel distance by leveraging advanced techniques such as K-means clustering, the nearest neighbor algorithm, and the 2-opt optimization technique.

## Features

- **Distance Calculation**: The code calculates the distances between state capitals using the Haversine formula in kilometers.
- **Clustering**: State capitals are grouped into clusters using the K-means clustering algorithm for better route management.
- **Nearest Neighbor Algorithm**: Within each cluster, the nearest neighbor algorithm is applied to find the most efficient route.
- **2-Opt Optimization**: The overall route is optimized using the 2-opt algorithm to reduce the total travel distance.
- **Unit Conversion**: The results can be easily converted between kilometers and miles, ensuring compatibility with different use cases.

## Project Structure

- **haversine()**: Function to calculate the distance between two geographical points using the Haversine formula.
- **nearest_neighbor_tsp()**: Implements the nearest neighbor algorithm to determine the optimal path within a cluster.
- **two_opt()**: Applies the 2-opt algorithm to further refine and optimize the route.
- **route_distance()**: Calculates the total distance of a given route.
- **K-means Clustering**: Groups state capitals into clusters for more manageable route optimization.
- **Final Route Calculation**: Combines optimized routes from all clusters and calculates the total travel distance, starting from Iowa (Des Moines) and ending at Washington, DC.

The script will output the final optimized route with the sequence of cities and the total travel distance: 26653.152279369275 km

