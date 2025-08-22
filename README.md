AutoGen Business Analysis Team
Overview
AutoGen Business Analysis Team is an AI-powered multi-agent system built with Streamlit, designed for comprehensive strategic business analysis. It integrates multiple specialized agents—Market Analyst, Financial Strategist, and Operations Manager—to provide in-depth insights, risk assessment, and actionable recommendations for business scenarios.

Features
Multi-agent collaboration orchestrated via AutoGen RoundRobin chat

Predefined and custom business scenario analysis

Market, financial, and operational insights with structured reporting

Executive summary and detailed report generation in markdown format

Interactive web UI allowing scenario selection, analysis history, and result exploration

Custom CSS styling for intuitive agent role visualization

Analysis history management with session persistence

Clear risk assessments and success metrics overview

Exportable reports for easy sharing and documentation

Getting Started
Prerequisites
Python 3.9 or higher

OpenAI API key

Install required packages:

bash
pip install streamlit autogen-agentchat autogen-ext python-dotenv
Setup
Create a .env file in the project directory and add your OpenAI API key:

text
OPENAI_API_KEY=your_api_key_here
Run the application:

bash
streamlit run your_script_name.py
Access the app at the URL provided by Streamlit.

Usage
Choose between predefined business scenarios or create a custom scenario by inputting company details, challenges, goals, and budget.

Click “Run Analysis” to trigger the multi-agent AI team.

View live analysis progress and examine results by agent role.

Generate and download executive summary or detailed markdown reports.

Manage previous analyses in the sidebar, with options to revisit or clear history.

Agent Roles
Agent Name	Icon	Responsibility
Market Analyst	📈	Market research, competitive analysis, trends
Financial Strategist	💰	Financial performance, budgeting, risk analysis
Operations Manager	⚙️	Process optimization, implementation planning
Technical Details
Multi-Agent Orchestration: Uses AutoGen RoundRobinGroupChat for turn-based agent communication with termination conditions (message count or explicit keyword).

OpenAI Model: Powered by GPT-4o-mini for agent responses.

Streamlit UI: Organizes workflow into tabs for analysis input, results display, and informational content.

Session Management: Stores analysis history and current analysis in Streamlit session state.

Report Generation: Constructs markdown-formatted executive and detailed reports from agent messages.

Styling: Custom CSS enhances readability and user experience.

Customization
Modify or extend agent system prompts for domain-specific adaptations.

Add additional predefined scenarios or customize UI text.

Adjust termination conditions or agent orchestration logic if needed.

Update UI styling and layout through the embedded CSS.

Troubleshooting
Verify your OpenAI API key is set correctly in environment variables or st.secrets.

Check network connectivity and API usage quotas if agents fail to respond.

Errors during analysis are displayed in the interface with details.

Clear analysis history if session state behaves unexpectedly.

License and Disclaimer
This project is intended for educational and demonstration purposes. Analyses generated are AI-assisted and should complement, not replace, professional consulting. Use responsibly.

Contact and Contributions
For issues, feature requests, or contributions, please refer to the project repository or contact the maintainers.
