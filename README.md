# photo-spotter-geo-service

## Table of Contents
- [Overview](#overview)
- [Planned Features](#planned-features)
- [Environment and Dependencies](#environment-and-dependencies)
- [API Endpoints](#api-endpoints)
- [Deployment and Usage](#deployment-and-usage)
- [Tasks](#tasks)

## Overview
This service manages geospatial data for photo spots. It provides storage and queries for location information (coordinates, bounding boxes, nearby searches).

## Planned Features
- Storage of coordinates and location metadata
- Nearby location queries
- Bounding box or region-based lookups
- Potential integration with third-party map APIs

## Environment and Dependencies
- Go or .NET 6+ for service logic
- PostGIS (PostgreSQL) or MongoDB for geospatial indexing
- Docker for container builds

## API Endpoints
- `/locations` for creating, reading, updating, and deleting location data
- `/locations/near` to find nearby points within a defined radius
- `/locations/bbox` to retrieve locations in a bounding box

## Deployment and Usage
- Run locally via `go run main.go` or `dotnet run` (depending on language)
- Build Docker image with `docker build -t photo-spotter-geo-service .`
- Deploy on Kubernetes using manifest files or Helm charts

## Tasks
- Scaffold CRUD operations for location data
- Implement geospatial queries
- Set up the continuous integration pipeline
- Provide a `/health` endpoint
