# Course Notes

**Note**: To mark this reading item as complete, make sure to scroll down to the end and click on "Mark as Complete".

## Claude Code Installation

To follow along with the lessons, here's how you can install Claude Code.

1. Run the following command:
    
    `npm install -g @anthropic-ai/claude-code`
    
    For more installation guides, you can find them [here](https://docs.anthropic.com/en/docs/claude-code/setup).
    

2. Once you have Claude Code installed, you can:
   - launch it from your terminal: navigate to your project folder & then type `claude`
   - launch it from the terminal integrated within VS Code by typing `claude`, the extension will auto-install. 
        - If you run into issues, ensure that `code` command is available. If not installed, use Cmd+Shift+P (Mac) or Ctrl+Shift+P (Windows/Linux) and search for “Shell Command: Install ‘code’ command in PATH”  
    
    For more info, check [Claude Code IDE Integrations](https://docs.anthropic.com/en/docs/claude-code/ide-integrations).


## Links to Course Codebase Examples

Here are the links to the coding examples covered in the lessons:

1. Codebase for the RAG chatbot (Lessons 2-6)
    - Here's [the repo](https://github.com/https-deeplearning-ai/starting-ragchatbot-codebase.git) of the starting codebase used in lesson 2.
    - Lessons 3-6 add features to the starting codebase.
    - Here's [the state](https://github.com/https-deeplearning-ai/ragchatbot-codebase.git) of the codebase after lesson 5.

    Feel free to fork the starting codebase and follow the lessons' activities.

2. E-commerce data analysis (Lesson 7)
    - Here are [the lesson files](https://github.com/https-deeplearning-ai/sc-claude-code-files/tree/main/lesson7_files).
    - It includes the data, the starting and refactored notebooks, and the dashboard file.

    Feel free to fork this repo, and try lesson 7 tasks using the starting notebook and the data folder.

3. Figma design mockup (Lesson 8)
   - Here's [the link](https://github.com/https-deeplearning-ai/sc-claude-code-files/blob/main/additional_files/key-indicators.fig) to the Figma mockup design (which you can open with [Figma Desktop App](https://help.figma.com/hc/en-us/articles/5601429983767-Guide-to-the-Figma-desktop-app)).
   - In lesson 8, you will build a Next.js app based on this mockup.
   - Here's the [link](https://github.com/https-deeplearning-ai/FRED-dashboard.git) to the repo of the app we got during filming.    


## Prompts and Summaries of Lessons

You can find the prompts used in each lesson and a summary of Claude Code features in the optional reading item at the end of the course. You can also find them in this [repo](https://github.com/https-deeplearning-ai/sc-claude-code-files/tree/main/reading_notes).


## Cost Visibility

If you'd like to install Claude Code to try the lessons:
- you can have a Pro (`$20`/month) or Max (`$100`/month) [subscription](https://www.anthropic.com/claude-code#:~:text=Pro,Sign%20up). The pro subscription is enough for the lessons' activities, but it doesn't include Opus. 
- Or, you can be billed based on API usage (if you just use sonnet for all the lessons' activities, the total cost for all lessons can be between `$12` and `$20`). In a given session, you can monitor the cost using the `/cost` command.