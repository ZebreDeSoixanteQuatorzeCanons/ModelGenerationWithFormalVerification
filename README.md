# Overview

This repository contains models generated with **TTool-AI**, using the feedback loop that integrates full syntax checking and model checking.

## Repository Structure

- **`./specifications/`** contains the specifications used to generate the models.  
- **`./models/`** contains the resulting generated models.

## Using the TTool-AI Feedback Loop

1. **Download TTool (v3.0 or later).**  
   We recommend downloading and compiling TTool from its public GitLab repository.  
   Download page: <https://ttool.telecom-paris.fr/download.html>

2. **Configure TTool for LLM integration.**  
   Follow the instructions given at <https://ttool.telecom-paris.fr/ttoolai.html>.  
   You will need either an OpenAI key, a MistralAI key, or a LLM server.

3. **Start TTool and create an AVATAR model.**  
   Launch TTool, create an empty AVATAR model (`Right-click > New Design`), then click the AI button to open the TTool-AI window.

4. **Generate and validate system blocks.**  
   In the `Selected chat` list, choose `Identify and validate system blocks`.  
   Paste your specification into the text field and click `Start`.  
   Once the interaction between TTool-AI and the LLM is complete, click `Apply response` to generate the validated block diagram.

5. **Generate and validate state machines and attributes.**  
   In the `Selected chat` list, select `Identify and validate state machine and attributes`.  
   Paste your specification again and start the interaction.
