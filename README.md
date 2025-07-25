# AI-Generated-LinkedIn-Content-Workflow-n8n-
This workflow automates the process of generating inspiring LinkedIn content by integrating Google Sheets, the Tavily API, OpenAI, and task tracking logic. It retrieves pending content tasks, collects research material, and produces original, high-quality posts using AI—marking tasks as complete when done.


# Workflow Overview
The system checks a Google Sheet for rows marked as "To Do" under a content task list. For the first pending task, it fetches related articles via the Tavily search API, feeds that context to an AI agent, and generates a creative and inspiring LinkedIn post. Once generated, the task status is updated from "To Do" to "Completed" in the sheet.


