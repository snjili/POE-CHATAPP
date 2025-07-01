# Cybersecurity Awareness Chatbot - README

## Overview
This application is a GUI-based Cybersecurity Awareness Chatbot designed to help users manage cybersecurity-related tasks, test their knowledge through quizzes, and receive reminders about important security practices. The chatbot features natural language processing simulation to understand user requests and maintains an activity log of all interactions.

## Features

### 1. Task Management
- Add cybersecurity-related tasks (e.g., "Enable two-factor authentication")
- Set optional reminders for tasks
- Mark tasks as complete
- Delete tasks
- View all active tasks

### 2. Cybersecurity Quiz
- 10 questions covering various cybersecurity topics
- Multiple-choice and true/false formats
- Immediate feedback with explanations
- Score tracking and final performance evaluation

### 3. Activity Log
- Records all significant actions (tasks, reminders, quiz attempts)
- Stores timestamps for each entry
- Displays last 10 activities by default
- Accessible via "Show activity log" or "What have you done for me?" commands

### 4. Natural Language Processing
- Understands variations of commands
- Extracts parameters from natural language input
- Handles different phrasings for the same request

## Installation

### Prerequisites
- .NET Framework 4.7.2 or later
- Windows OS (for Windows Forms/WPF application)

### Steps
1. Clone the repository:
   ```
   git clone https://github.com/yourusername/cybersecurity-chatbot.git
   ```
2. Open the solution file in Visual Studio
3. Build the solution (Ctrl+Shift+B)
4. Run the application (F5)

## Usage

### Starting the Chatbot
1. Launch the application
2. The chatbot will greet you with: "Welcome to Cybersecurity Awareness Chatbot! How can I help you today?"

### Adding a Task
- Type: "Add task to review privacy settings"
- The chatbot will confirm and ask if you want a reminder
- To set a reminder: "Yes, remind me in 3 days"

### Taking the Quiz
- Type: "Start cybersecurity quiz"
- Answer each question by typing the letter of your choice
- Receive immediate feedback after each answer
- View your final score at the end

### Viewing Activity Log
- Type: "Show activity log" or "What have you done for me?"
- The chatbot will display your recent activities

## Examples

### Task Management
```
User: Add task to update all passwords
Chatbot: Task added: 'Update all passwords'. Would you like to set a reminder for this task?
User: Remind me in 14 days
Chatbot: Reminder set for 'Update all passwords' in 14 days.
```

### Quiz Interaction
```
Chatbot: Question 1: What should you do if you receive an email asking for your password?
A) Reply with your password
B) Delete the email
C) Report the email as phishing
D) Ignore it
User: C
Chatbot: Correct! Reporting phishing emails helps prevent scams.
```

### Activity Log
```
User: What have you done for me?
Chatbot: Here's a summary of recent actions:
1. [2023-11-15 14:30] Task added: 'Update all passwords' (Reminder set for 14 days)
2. [2023-11-15 14:25] Quiz completed - Score: 8/10
3. [2023-11-15 14:15] Task marked complete: 'Enable two-factor authentication'
```

## File Structure
```
CybersecurityChatbot/
├── MainWindow.xaml        # Main application window
├── Models/
│   ├── TaskItem.cs        # Task data model
│   ├── QuizQuestion.cs    # Quiz question model
├── Managers/
│   ├── TaskManager.cs     # Task management logic
│   ├── QuizManager.cs     # Quiz logic
│   ├── NlpProcessor.cs    # NLP simulation
├── Utilities/
│   ├── ActivityLog.cs     # Activity logging system
├── Resources/             # Contains images and other resources
```

## Troubleshooting

### Common Issues
1. **Application won't start**: Ensure you have the correct .NET Framework version installed
2. **Commands not recognized**: Try rephrasing your request or use more specific keywords
3. **Quiz questions not displaying**: Verify all quiz questions are properly initialized in QuizManager.cs

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your improvements.

## License
This project is licensed under the MIT License.
