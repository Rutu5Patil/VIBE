<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Automate Your Calendar with AI

**Project Link:** [View Project](http://learn.nextwork.org/projects/ai-agent-nocode)

**Author:** naru uzu  
**Email:** rutu13patil@gmail.com

---

---

## Introducing Today's Project!

🔧 Set up an AI workflow using n8n.

🤖 Integrate ChatGPT and Google Calendar into your workflow.

⚙️ Configure dynamic expressions and a system message for accurate scheduling.

💎 Secret Mission: Customize your AI assistant's personality with prompt engineering. 


### Key tools and concepts

🔧 Use n8n to build a workflow.

🤖 Integrate ChatGPT as your AI model to understand requests.

🗓️ Integrate Google Calendar as your calendar tool

⚙️ Configure dynamic expressions and system messages for accurate scheduling.

💎 Change your AI's personality with advanced system messages.

* Added 2 more Google Tools for keeping track of event ID and for deleting events.


### Challenges and wins

This project took me little time only. The most challenging part was adding a delete event tool cause for it I had to add a tool to keep track of events/finding eventid.

### Why I did this project

I did this project today to learn how to work with n8n.

---

## Exploring n8n

Sign up to n8n

Explore the n8n workspace

![Image](http://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/ai-agent-nocode_c9d8f7a2)

---

## Starting an AI Workflow

In this step:

Create a new workflow in n8n
Add a chat trigger to the workflow
Test the chat trigger

A workflow is a chain of tools and actions that we automate. 

![Image](http://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/ai-agent-nocode_a4b3c2d1)

### Understanding workflows

A workflow is a set of steps that complete a task; automating it means those steps run on their own, which saves you time and reduces errors.

A workflow becomes an AI workflow when it uses AI to automate tasks or decisions. For example:

Using image recognition to sort and categorize photos you upload to a folder.

Using generative AI to automatically draft a reply to new emails in your inbox.

### Configuring workflow triggers

A workflow trigger is like a starting point for a workflow.

It's what tells the workflow to begin. It can be something that happens at a specific time, like every hour, or something that happens because of an event, like getting a new email.

---

## Integrating ChatGPT

Add an AI Agent node to your workflow.

Connect an OpenAI Chat Model.

![Image](http://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/ai-agent-nocode_fmtkjyrg)

### Connecting AI agents

The node is called AI Agent, but we're building an AI workflow: it runs when you send a chat message (a trigger), not on its own. A true agent decides when to act without a trigger.

### Key components of an AI workflow

An AI agent is made of three key parts that you set up individually:

The Chat Model is the AI agent's brain, trained to analyze data to make decisions.

The Memory section stores data, past interactions, and learned information. This helps the AI agent learn from its past experiences and make better decisions over time.

The Tool section is the third-party software your agent will use. You can also use tools to enhance your AI agent, like using tools that help the AI communicate and speak in a different language.

![Image](http://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/ai-agent-nocode_o5p6q7r8)

### Choosing the AI model

OpenAI offers different AI models. Each model is made for different jobs. Some models are good at simple tasks like finishing sentences, while others are better at complex tasks like understanding conversations. We'll be using their simplest model, which still works perfectly for simple tasks like creating calendar events.

gpt-4o-mini

This is a highly reliable, fast, and cost-efficient lightweight model. It is excellent at processing structured data, interpreting calendar dates, and handling basic JSON formatting. Because it is the model recommended in our project instructions, selecting this keeps everything perfectly aligned with the screenshots and guidelines.

---

## Integrating Google Calendar

Add a connection to Google Calendar.

Set up dynamic expressions for event scheduling.

![Image](http://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/ai-agent-nocode_c9d8dfgv2)

### Understanding tools in AI workflows

A Tool is a piece of code or third party software that the agent can use to do a task.

Tasks could include retrieving data from a database, or in our case, creating an event in an external calendar (Google Calendar).

### Security considerations for integrations

This authorization lets your workflow act on your behalf, adding and checking events in your Google Calendar.

Without this authorization, your workflow can't access your calendar or do its job.

---

## Configuring Dynamic Expressions

$fromAI() expressions tell the Calendar tool to get its values from the AI model, instead of using hardcoded defaults. The parameter name inside (like start_time) is a hint to the AI model about what information to look for in the chat.

For example, $fromAI('email') would make the AI model look for an email address instead of a time.

![Image](http://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/ai-agent-nocode_897rg465e)

---

## Writing a System Message

Add a system message to your AI agent.

Configure the system message to use Expression mode.

![Image](http://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/ai-agent-nocode_rfgdhn456)

### Understanding system messages

The system message is a prompt that your workflow sends to the AI agent before it starts processing your chat message.

If you don't enter a system message, your AI agent doesn't have any instructions on what it's meant to do and the current context (e.g. today's date).

---

## Testing the Workflow

Test your AI workflow with a chat message.

Verify the calendar event was created at the correct time.

![Image](http://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/ai-agent-nocode_w3x4y5z6)

### Verifying the results

A meeting is scheduled at the right time. Your AI-powered calendar assistant is working!

---

## Changing My AI Agent's Personality

Change how your calendar assistant talks and books meetings.

Showcase advanced prompt engineering skills in your documentation!

### Updating system messages

In the n8n workflow's canvas, double-click on your AI Agent. Clear everything that's inside the System Message window.
Now let's add new prompt inside:

### Observing agent behavior changes

Advanced system messages to transform the assistant's tone, add custom rules, and could see just how much control prompt engineering gives you over AI behavior.


### Adding constraints with system messages

This system message programs your AI agent to follow unique rules: meetings must start at prime-numbered minutes and can only be booked on even-numbered days.

This assistant will also check your mood before scheduling. Do you feel like doing the meeting?

Let's put it to the test. If it works, you'll see how system messages can do more than change your AI agent's tone of voice. You can also add constraints like only allowing certain event times!

![Image](http://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/ai-agent-nocode_fewargtr52)

---

---
