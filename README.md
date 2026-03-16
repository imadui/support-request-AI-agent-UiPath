# Support Request Handling Agent

This is a full agentic automation project: **Support Request Handling Agent**.

## Overview

The process starts by checking a source directory for any support request files.  
If files are found, they are downloaded and written in **JSON** format.

The workflow then extracts the request message using a **JSON deserialization** method.  
After that, the message is analyzed by an **agent powered by GenAI** to determine the category of the request.

The possible categories are:

- **Deposit**
- **Withdraw**
- **Product**

Based on the detected category, the file is automatically moved to a specialized directory so it can be handled by the appropriate team.

## Process Flow

1. Check the source directory for incoming support request files.
2. Download and convert the files into JSON format.
3. Extract the request message through JSON deserialization.
4. Send the request message to the GenAI agent for classification.
5. Identify the request category:
   - Deposit
   - Withdraw
   - Product
6. Route the file to the corresponding specialized directory.
7. Allow the correct team to process the request.

## Purpose

The goal of this project is to automate the triage and routing of support requests using agentic automation and GenAI, reducing manual effort and improving response efficiency.

## Project Structure

- `01 Data` – input and processed data files
- `02 StudioWorkflows` – UiPath workflows
- `03 Source_Directory` – source files to be checked and processed
- `Support-Request-handler.bpmn` – BPMN model of the process
- `System Prompt.txt` – prompt used by the agent
- `support-request-handler.uis` – related project file

## Technologies Used

- **UiPath**
- **GenAI / AI Agent**
- **JSON Deserialization**
- **BPMN**
- **File-based routing automation**

## Author

**Imad Eddine**
