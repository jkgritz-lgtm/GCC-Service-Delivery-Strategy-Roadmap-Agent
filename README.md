1. Overview
Agent Name: GCC Service Delivery Strategy
Deployment Platform: Gemini Enterprise
Description: An AI agent designed to generate a comprehensive Service Delivery Strategy roadmap based on user-uploaded documents and interactive chat inputs, outputting the final deliverable as a Google Slides presentation.
Primary Business Goal: To streamline, standardize, and accelerate the creation of structured Service Delivery Strategy roadmaps for customers.
2. Target Audience & Personas
Primary Users: Service Delivery Managers, Consultants, and Account Executives.
3. Core Functionality & Workflow
Core Tasks:
Ingest and analyze user-uploaded context documents and chat inputs.
Extract key information mapping to required roadmap sections.
Identify data gaps and proactively ask the user clarifying questions.
Formulate and propose industry-standard assumptions to fill gaps when necessary.
Format and generate a fully structured Service Delivery Strategy roadmap as a Google Slides presentation.
Ideal Workflow:
User initiates the session by providing context via chat and uploading relevant documents.
Agent analyzes the input against the required sections.
Agent identifies missing information, asks targeted clarifying questions, and suggests industry-standard assumptions.
User responds with clarifications or approves assumptions.
Agent synthesizes all data, maps it to slide layouts, and generates the final Google Slides presentation.
4. Technical Specifications
Model Selection: gemini-3.1-pro-preview (Best suited for deep reasoning, complex document analysis, and strategic formulation).
Data Sources:
User Uploaded Documents (PDFs, Docs, Spreadsheets)
Direct Chat Context
Required ADK Tools:
google_slides_generator: Integrates with Google Workspace/Slides API to programmatically create and format a Google Slides presentation from the agent's structured output.
5. Output & Delivery
Format: Google Slides Presentation
Required Output Sections (Slides):
Vision
Services Delivery Strategy
Commercials
Delivery Approach
Roles & Responsibilities
Operating Model (PSO only, Partner, or both)
6. Edge Case Handling
Missing Information: If data for a specific section is missing, the agent will pause final generation, ask the user targeted clarifying questions, and offer industry-standard assumptions for the user to approve or modify.
7. Success Criteria & Metrics
KPIs:
Significant reduction in the time required to draft delivery strategy presentations.
High user acceptance rate of generated presentations with minimal manual rewrites.
Acceptance Criteria: The final output must be delivered as a formatted Google Slides presentation explicitly containing slides for all required sections and demonstrate the ability to intelligently prompt the user for missing info before finalizing.
8. Security & Permissions
Enterprise-grade data privacy per Gemini Enterprise standards.
Session-scoped data handling ensuring uploaded customer documents remain secure and transient.
Requires Google Workspace OAuth permissions to create and save Slides on the user's behalf.
