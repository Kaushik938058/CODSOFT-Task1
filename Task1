\*The primary goal of this task is to develop a functional chatbot that utilizes rule-based responses to interact with users. This project serves as an introduction to the basic concepts of natural language processing and the logical flow of digital conversations.
How the Code Works
The chatbot is built using Python and the re library, which allows for sophisticated pattern matching techniques to identify specific user queries. The program begins by capturing user input and converting it to lowercase to ensure the matching process is not affected by capitalization. It then compares the user's words against a dictionary of predefined rules using a loop.
When a match is found between the user's input and a stored pattern, the chatbot triggers a specific, appropriate response. For example, if the user mentions "AI" or "Artificial Intelligence," the script is programmed to provide a clear definition of the field. If the user provides an input that does not match any of the established rules, the chatbot returns a default message asking for clarification.
Technical Implementation
The system relies on a series of if-else statements and regular expression searches to manage the conversation flow. This logic ensures that the AI agent remains predictable and provides accurate information based on the instructions provided. Following the internship guidelines, this project has been uploaded to a dedicated GitHub repository named CODSOFT to showcase professional diligence and technical progress*/


import re

def chatbot_response(user_input):
    # Convert input to lowercase for consistency
    user_input = user_input.lower()

    # Define rules and responses (Pattern Matching)
    # Each key is a regex pattern, and the value is the AI's reply
    rules = {
        r'hi|hello|hey': "Hello! I am your CodSoft AI assistant. How can I help you?",
        r'what is your name': "I am a Rule-Based Chatbot created for my AI internship.",
        r'how are you': "I'm doing well! I'm here to help you with your tasks.",
        r'what is (ai|artificial intelligence)': "AI is the simulation of human intelligence by machines.",
        r'help': "I can answer basic greetings and questions about AI. Try asking 'What is AI?'",
        r'bye|goodbye': "Goodbye! Best of luck with your CodSoft internship!"
    }

    # Iterate through rules to find a match
    for pattern, response in rules.items():
        if re.search(pattern, user_input):
            return response

    # Default response if no pattern matches
    return "I'm sorry, I don't understand that. Could you try rephrasing?"

# Main interaction loop
print("--- CODSOFT AI INTERNSHIP: TASK 1 (CHATBOT) ---")
print("Type 'bye' to exit the conversation.\n")

while True:
    user_text = input("You: ")
    
    # Exit condition
    if re.search(r'bye|goodbye', user_text.lower()):
        print("Chatbot: Goodbye!")
        break
        
    print(f"Chatbot: {chatbot_response(user_text)}")
