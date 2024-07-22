<p align="center">
    <img src="./assets/Logo.png"  width=25% height=25%>
</p>


# Welcome to the Feedback Bot Project!

I developed this during my internship at TomTom.
It aims to automate managing feedback across multiple Slack channels. It was built with the Slack Bolt framework in Python.
This bot reduces manual intervention by categorizing feedback using AI, storing it in a database, generating Jira tickets, and visualizing data through Grafana dashboards.

## Problem Statement

The current method of processing feedback from the Slack channel is manual. It involves individual replies to users and creating Jira tickets with attachments. This manual process makes it challenging to effectively track issues related to specific components.

## Features

- **Feedback Parsing:** Analyze Slack messages to determine the number of incidents per message, extract titles, and discern the domain or category of feedback such as Routing, Guidance, Map Visualization, and Search using a trained Large Language Model (LLM).
- **Multi-Channel Capability**: Designed to operate across multiple Slack channels.
- **Integration with JIRA**: Each categorized feedback item automatically propagated as a new ticket to JIRA via the JIRA API.
- **Development of a Grafana Dashboard:** Develop a dashboard to visualize and monitor feedback data effectively.

## Technologies Used

- **Framework**: Slack Bolt for Python.
- **Machine Learning**: Used OpenAI's API and prompt engineering to:
  - **Incident Analysis**: To create a specific system message that enables the LLM to determine the number of incidents reported within a single feedback message.
  - **Title Generation and Categorization**: Automatically generates titles for each incident and categorizes them based on predefined criteria such as (Routing, Guidance, Map Visualization, and Search).
- **Database**: PostgreSQL.
- **Database Migration**: Flyway.
- **Visualization**: Grafana Dashboard.
- **Deployment**: Azure Container Apps.

#### Workflow overview:
<p align="center">
    <img src="./assets/workflow.png"  width=70% height=70%>
</p>

## What I Learned

This project was an invaluable learning experience. It covered a range of technical, organizational, and design challenges that contributed significantly to my professional growth.

- **Collaborative Teamwork**: Collaborated closely with other teams to deliver the best solution and address their requirements.
- **Project Management**: Advanced my project management skills using JIRA to create tickets, organize epics, prioritize components, and track issues, using Confluence for comprehensive project documentation.

- **Technical Skills**:
  - OpenAI and Prompt Engineering.
  - Slack Bolt framework.
  - Docker.
  - Databases and migrations (PostgreSQL, Flyway).
  - Jira API and Grafana Integration.

This project improved my technical capabilities and reinforced the importance of clear communication, thorough documentation, and user-focused design in software development. 

