##The Easiest Part of the Application

#Context:
Generates a compact summary of the project that can be understood by artificial intelligence.

#Context IA:
Uses Gemini to generate a summary of your project. The first time you run it, it will ask for an API key, which you can obtain easily and for free at: https://ai.google.dev/aistudio.

##The Slightly More Difficult Part: Generating Custom Contexts

**A context is simply a list of files.**

You can define a new context or switch to an existing one using:
**context check <context_name>**
This will also display the contents of the context.

You can add new files to your current context with:
**context add <file_path>.**

You can list all the contexts in your .context directory with:
**context list.**

You can define which fragments of each file are displayed in each context by including the tags:
CONTEXT_{context_name}_START
CONTEXT_{context_name}_END
within your file as many times as needed.

**Context Init:**
By default, the contexts you create are saved in a global folder. context init allows you to create a local .context folder that you can upload to your git repository.

Context Help or Context H:
Displays help information and the available commands.
