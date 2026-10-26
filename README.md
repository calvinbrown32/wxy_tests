# wxy_tests

This is a brief assignment to assist in the hiring process for urban analysts at WXY. Please complete parts A, B and C below. Please clone this branch and send us back a link to a repo with answers to parts A & C in a markdown file & a notebook that shows your work on part B. 

Please do not spend more than two-three hours on this assignment. We do not want you to go overboard! 

Please do not us AI for this exercise. We use AI in some contexts, but this is about your approach, how you frame problems, and your coding style. We want to see how you think and how you work.

## A. Web Development 


1. Please share a link to a code base for a website you have built or substantively contributed to. If it was a collaboration please provide a clear description of your role. 

------------------------------
Calvin's Response:

Hello, below is the GitHub link to a Replica data parser I built that quickly turns Replica mobility data into an interactive origin-destination flow map using FlowMapBlue, an open source tool. David Wasserman presented his idea for using Replica data and FlowMapBlue to create an interactive O-D flow viewing tool, and intrigued I went home and started building it! 
- https://github.com/calvinbrown32/Replica_Parser

Link to a demo of the tool and a detailed description of the project:
- https://calvinbrown.pythonanywhere.com

Also, I wanted to share my code base to a fully built and deployed React app I built. The app runs on React,React Leaflet, and a postgres backend and is deployed on a Digital Ocean Droplet. I realized there might be items in the repository that I don't want to share, but I can share a link to the app:

- http://174.138.79.56/seating/
- username: cbrown
- password: cbrown
------------------------------

1. In no more than a few paragraphs, please describe how you would approach developing a website for the scenario described below. Feel free to include simple diagrams of the architecture as helpful.  We want to understand how you approach system design in web development, the tools you are familiar with, and how you would approach this problem from start to finish. Feel free to add additional detail on parts where you have strong opinions or experience, including libraries, frameworks, and best practices. Feel free to do research; however, we are most interested on you drawing on your own experience and knowledge, and the specific benefits or challenges your experience would lend in addressing this problem.

    You are working with the NYC Department of City Planning on a neighborhood plan. As part of the process, we are developing a website to solicit community input on what the plan should include. The website must have an interactive map with context layers and a feature that allows community members to add  comments to the map to share ideas for the plan. The comments should not be publicly visible on the site but must be saved along with their location information so that they can later be analyzed. 


========================
Calvin's Response:

This sounds like a really interesting project. I would start by breaking it down into three core components:

1. Client Coordination: Work closely with DCP to understand their needs, expectations, and minimum requirements, ensuring that the project scope and priorities are clearly defined from the outset.

2. System Design: Establish a reliable technical architecture that supports the site's core functionality. My strongest experience is with React and React-Leaflet on the front end, paired with a PostgreSQL/PostGIS backend to store user data and spatial layers for interactive mapping. I've built similar applications and would leverage those existing approaches while adapting them to the project's specific needs. I've also worked with more turnkey solutions, such as Felt, where appropriate.

I also have experience developing community engagement maps and understand the importance of carefully designing how users create spatial features and associate comments with locations on a map. For example, requiring users to zoom in to an appropriate scale before placing a point or drawing a feature can help ensure that contributions are accurately located. These seemingly small design decisions can make a significant difference in the quality and usability of the data collected.

3. Visual Design and User Experience: Design an intuitive experience that guides users through the entire journey, from accessing the website and creating an account to exploring the map, submitting comments, and returning to saved contributions in later sessions. I'd focus on making the available tools and options easy to understand, with clear visual guidance and help resources accessible throughout the experience.
========================


## B. Geospatial Python Test

Please analyze and visualize Active Major Construction permits in New York City in a jupyter notebook (New Building or Major Alteration A1). The data can be downloaded [here](https://data.cityofnewyork.us/Housing-Development/DOB-Permit-Issuance/ipu4-2q9a).

At a minimum:

- Load and clean the data, demonstrate you have a grasp of the data and its contents
- Create a summary table with key metrics
- Visually explore key metrics through graphs 
- Perform a spatial join against another layer of your choice (e.g. Census layers, transit walksheds, etc.)
- Create a summary table making use of the joined data points
- Export one graph and one chart that are presentation-ready or could be slightly refined in Adobe CC 
- Export your final data to excel
- In the final cell(s) of the notebook, indicate your assumptions, the research questions you were pursuing, and what your analysis revealed.

The objective of this question is to get a flavor for your coding style and analytical approach. Please don't spend more than 1-2 hours on the assignment. We will run the notebook, so make sure it can be run sequentially!

None of your code will be used by WXY for project work.

## C. Use of LLMs

In a brief paragraph please describe any experience you have to date using large language models (LLMs) for code development and/or refinement. Please describe use cases you have encountered in your work and how you have approached using these tools. 

========================
Calvin's Response:

I now use LLMs for approximately 90% of my code development and refinement. I instruct LLM tools to use libraries and methods that I have been using for nearly a decade, long before LLMs became widespread. This allows me to accelerate development, troubleshoot errors, and refine existing workflows while maintaining code quality, functionality, coherence, and my own understanding of the underlying code and logic.
========================

