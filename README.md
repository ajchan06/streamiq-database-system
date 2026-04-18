# StreamIQ – Music Streaming Database System

## Overview
StreamIQ is a relational database system designed for a music streaming platform. It models core entities such as users, artists, albums, songs, playlists, and listening history, while supporting analytics, recommendations, and royalty tracking.

The system captures complex real-world relationships and logs every play event, enabling data-driven insights into user behavior and platform performance.

---

## Key Features
- Fully normalized relational schema (BCNF)
- Complex relationship modeling (many-to-many, ordered data)
- Playlist system with song ordering
- User–artist follow relationships
- Playback tracking for analytics and recommendations
- SQL-based implementation with enforced constraints

---

## System Design

### Core Entities
- Users  
- Artists  
- Albums  
- Songs  
- Playlists  
- Listen History  

### Key Relationships
- Users follow artists  
- Songs belong to albums  
- Songs have multiple contributing artists (many-to-many)  
- Playlists contain ordered songs  
- Users generate listening events  

---

## Database Architecture

The system was designed using:
- UML Class Diagrams  
- Entity-Relationship Diagrams (ERD)  
- Functional dependencies  

The schema is:
- Normalized to Boyce-Codd Normal Form (BCNF)  
- Designed to eliminate redundancy  
- Structured to maintain strong data integrity  

---

## Implementation

Implemented in SQLite with:

- Primary keys for unique identification  
- Foreign keys for relational integrity  
- Domain constraints for validation  

The database supports:
- Efficient querying  
- Scalable data relationships  
- Analytics-ready structure  

---

## Analytics Capabilities

The system enables:
- Monthly listening summaries  
- User behavior analysis  
- Recommendation-ready data structures  
- Royalty attribution based on play events  

---

## Project Structure

streamiq-database-system/  
├── db_requirements/  
├── db_schemas/  
├── diagrams/  
├── queries/  
├── screenshots_sql_def/  
├── streamiq-bonus-app/  
└── README.md  

---

## Diagrams

UML Diagram:  
https://lucid.app/lucidchart/c9bd40e4-83f2-448a-9769-c81f1e9cafdc/edit  

ER Diagram:  
https://lucid.app/lucidchart/2494d36e-d23b-486d-ba1d-4e3ead02742b/edit  

---

## What I Learned
- Designing scalable relational database systems  
- Applying normalization (up to BCNF)  
- Modeling complex real-world data relationships  
- Translating conceptual models into SQL schemas  
- Structuring data systems for analytics and performance  

---

## Future Improvements
- Build a backend API (Node.js / Express)  
- Integrate Redis for caching and real-time performance  
- Add recommendation algorithms  
- Develop a frontend dashboard for visualization  

---

## Tech Stack
- SQLite  
- SQL  
- UML / ER Modeling  

---  

## AI usage disclose
I used ChatGPT (GPT-5.2) as a development assistant to review and refine my UML diagram structure, helping me correct multiplicities, relationships, and overall model consistency before translating it into a relational schema. The model also assisted in generating sample test data and SQL table definitions, which I reviewed, adjusted, and validated to ensure they met the project requirements and normalization standards.

---

## Author
Anthony Chan  
Computer Science, Northeastern University
