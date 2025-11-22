🍳 AI-Powered Recipe Generation Workflow
Automated with n8n + OpenAI + Custom Website

This repository contains a complete AI-driven Recipe Generation System built using n8n (workflow automation) and the OpenAI Chat Model. The system takes a user’s recipe prompt from a website, processes it automatically, generates a structured recipe using AI, and returns the result instantly — all in real time.

This project demonstrates how automation and artificial intelligence can work together to create fast, efficient, and user-friendly recipe generation.

🚀 Features
✅ Automated Recipe Generation

Users can enter any cooking-related prompt (e.g., “Chicken Biryani”, “French Fries Recipe”), and the system instantly generates:

Ingredients

Step-by-step instructions

Optional variations or tips

✅ Real-Time Workflow

Triggered directly from the website via a webhook, the system processes the request and responds within seconds.

✅ Clean Text Extraction

Before sending the input to the AI model, the workflow extracts and cleans the user’s prompt to ensure accuracy.

✅ Structured Output

The workflow returns a clean, user-friendly recipe ready to display on any frontend.

🧠 Workflow Overview
1. Webhook Trigger Node

The user submits a recipe prompt on the website.
This fires a Webhook Trigger node in n8n, initiating the workflow.

2. Extract Prompt Node

The incoming request contains metadata from the website.
This node isolates only the user’s actual recipe text.

3. Recipe Agent (OpenAI Chat Model)

The cleaned prompt is sent to the OpenAI Chat Model.
The AI generates a full recipe, including ingredients and instructions.

4. Clean Generated Response Node

The recipe response may include unwanted characters or formatting.
This node cleans and prepares the final recipe text.

5. Webhook Response Node

The cleaned recipe is returned directly to the website as the final result.
The process is seamless and happens in real time.

🗂️ Suggested Folder Structure
/n8n-recipe-generator
   ├── workflow.json
   ├── README.md
   └── screenshots/
        └── <img width="905" height="362" alt="Screenshot 2025-11-22 131413" src="https://github.com/user-attachments/assets/3043feb9-cca6-416e-a8ec-fd58a08b2072" />


🛠️ Technologies Used
Tool	Purpose
n8n	Automation workflow
Webhook Trigger / Response	Communication with website
OpenAI Chat Model	Recipe text generation
JavaScript / Set nodes	Data cleaning and formatting
Custom Website	User interface for entering prompts
🎯 Use Cases

Recipe generator apps

AI cooking assistants

Food blogs

Restaurant menu creation tools

Learning platforms

📌 Advantages

Fully automated — no manual effort needed

Clean and professional recipe formatting

Easy to integrate with any frontend

Fast and scalable

Works in real time

📸 Demo (Optional)

Include screenshots of:

Webhook trigger

Extract prompt node

Recipe agent output

Frontend result

📢 Future Enhancements

Multi-language recipe generation

Nutrition estimation

Additional formatting styles

Support for vegan, halal, keto-specific recipes

Integration with image generation (future version)

🤝 Contributions

Contributions and suggestions are welcome.
Feel free to open issues or submit pull requests.

📬 Contact

Created by Tanzeela Sharif
For queries or collaboration: your email / LinkedIn link here
