Name:Kaushik
Company:CODSOFT
ID:BY25RY255105
Project Title: Chatbot with Rule-Based Responses
Domain: Artificial Intelligence

OVERVIEW OF THE PROJECT
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Objective
The primary goal of this project is to build a simple chatbot that interacts with users by processing inputs and generating responses based on a predefined set of rules. This project aims to demonstrate a fundamental understanding of Natural Language Processing (NLP) and conversation flow.

Technical Implementation
This chatbot is built using Python and relies on the re (Regular Expressions) module to handle text processing.
Pattern Matching: The core logic uses if-else statements and regular expressions to detect specific keywords or phrases in the user's input.

Response Mechanism:
Normalization: All user input is converted to lowercase to ensure consistency and case-insensitivity (e.g., treating "Hello" and "hello" as the same).
Rule Set: A dictionary maps specific regex patterns (keys) to their corresponding AI responses (values).
Fallback Handling: If the user's input does not match any defined rules, the bot triggers a default "I don't understand" response to maintain the conversation flow.

Key Features
Simple Interaction: Handles basic greetings, questions about the bot's identity, and inquiries about AI.
Robust Matching: Uses logical OR operators (e.g., hi|hello|hey) to catch various phrasing of similar intent.
Exit Condition: Includes a specific rule to detect "bye" or "goodbye" to gracefully terminate the conversation loop
