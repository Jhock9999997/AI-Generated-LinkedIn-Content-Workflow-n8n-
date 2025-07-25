# AI-Generated-LinkedIn-Content-Workflow-n8n-
This workflow automates the process of generating inspiring LinkedIn content by integrating Google Sheets, the Tavily API, OpenAI, and task tracking logic. It retrieves pending content tasks, collects research material, and produces original, high-quality posts using AI—marking tasks as complete when done.


# Workflow Overview
The system checks a Google Sheet for rows marked as "To Do" under a content task list. For the first pending task, it fetches related articles via the Tavily search API, feeds that context to an AI agent, and generates a creative and inspiring LinkedIn post. Once generated, the task status is updated from "To Do" to "Completed" in the sheet.

<img width="1674" height="528" alt="image" src="https://github.com/user-attachments/assets/bb75eb6b-08d8-4363-868c-b3a5435a095c" />

# Step-by-Step Process

1. Manual Trigger
The workflow is executed manually by clicking the "Execute Workflow" trigger node.

2. Read Google Sheet
The system retrieves rows from a designated Google Sheet that lists pending content tasks.

<img width="1344" height="1348" alt="image" src="https://github.com/user-attachments/assets/53040021-1fc5-42ab-b50d-f45811034116" />



4. Tavily HTTP Request
For the first task, it makes a POST request to the Tavily search API to retrieve three relevant articles based on the task topic or query.

5. AI Agent (OpenAI)
The AI agent consumes the collected research material and generates an inspiring, creative, and professional LinkedIn post tailored to the input.

6. Update Google Sheet
Once the content is generated, the corresponding row in the Google Sheet is updated—marking the task as “Completed.”

# Use Case
This workflow streamlines the content creation process for marketing or personal branding. It eliminates manual research and writing by allowing the AI to produce insightful, high-quality LinkedIn posts from curated source material, all while maintaining a clear task tracking system


