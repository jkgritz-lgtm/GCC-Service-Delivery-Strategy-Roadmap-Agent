# GCC Service Delivery Strategy

An AI agent deployed on Gemini Enterprise designed to generate a comprehensive Service Delivery Strategy roadmap based on user-uploaded documents and interactive chat inputs, outputting the final deliverable as a Google Slides presentation.

## Architecture

This multi-agent system comprises:
- **GCC_Service_Delivery_Strategy_Agent**: The main orchestrator.
- **GCC_Service_Delivery_Strategy_Pipeline**: A SequentialAgent that guides the process.
- **DocumentAnalyzerAgent**: Analyzes context docs and identifies gaps.
- **StrategySynthesizerAgent**: Formulates strategy sections and prompts the user for missing information.
- **SlidesGeneratorAgent**: Structures finalized content and generates Google Slides via tools.

## Tools
- `document_reader`: Utility tool for reading and parsing uploaded documents.
- `google_slides_generator`: Simulates API interaction to generate a Google Slides presentation from structured JSON.
