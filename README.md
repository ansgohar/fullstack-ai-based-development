# fullstack-ai-based-development

## Technology Stack:

### Supabase

- Database
- Authentication
- Storage
- Vault

### Frontend

- NEXT.js 16
- Tailwind CSS
- Shadcn UI

### Backend

- Java
- Spring Boot
- PostgreSQL
- JWT

## Prompt Requirements:

| Task                  | Tool                                  | Model            |
| --------------------- | ------------------------------------- | ---------------- |
| Project Management    | ChatGPT                               | GPT 5.2 Thinking |
| Front End Development | Antigravity                           |                  |
| Back End Development  | VS Code + (Claude <br>+ GLM)          |                  |
| Code Review           | CodeRabbit                            |                  |
| Containerization      | Docker + Podman                       |
| Deployment            | AWS EC2 **OR** Bunny Magic Containers |

## Install Spec-kit

https://github.com/github/spec-kit

## Prompt Engineering

### Prompt for the ChatGPT :

<!-- #### [Prompt](prompt_chatgpt.md) -->

#### Prompt Step 1 (Prompt):

Create a project and prepare an implementation plan using the spec-kit. Here is the project brief:
We're building Todo AI App. Domain is todoai.app. It is a multi-tenant saas toda and task managment app.
Next.js 16 + Spring Boot + Supabase (Auth, DB, Vault, Storage)
User can create multiple goals.
For each goal user can create multiple task lists.
Task List Management

- User can create tasks
- User can edit tasks
- User can delete tasks
- User can mark tasks as completed
- User can mark tasks as incomplete
- User can set due dates for tasks
- User can set reminders for tasks
- User can set priority levels for tasks
- User can set status for tasks

Brand kit customization
Admin analytics dashboard
Hosted on Bunny Magic Containers

You will act as a project manager. Code will be written using Claude Code and GLM 4.7. Also, the frontend code will be done using AntiGravity (using Gemini 3 pro).

Your task is to provide us with the plan, specs as we're going to use spec-kit (look it up).

<!-- Dont forget that We can have ONE specification. -->

We need to have multiple specifications. For example, we'll have 3 main areas to work on,

1. Database setup
2. Backend work
3. Fontend.
   I don't want the /specify commands from you now, however,
   I need a complete implementation that we'll extract specifiation latter.

Ask me any questions for clarification BEFORE we start.

#### Prompt Step 2:

- Need to answer the prompt questions and create specs.
- Copy the constitution to the clipboard from the constitution.md file.

#### Prompt Step 3:

run Claude code
//run claude inside the terminal in plan mode

```bash
claude code
```

Now run this

```bash
claude /speckit.consistution (past the constitution here)
```

or Press `command + J` and select `/speckit.consistution` and paste the constitution here.
save file

#### Prompt Step 4:

- Open VS Code and run claude in plan mode and start with the below prompt
  This is the implementation plan I got from ChatGPT. I want you to revise carefully and then we work together and you use the questions tool you have to interview for anytging that is not clear to you.
- past the plan inside this file and then answer the existed questions.
- add the following text
  Saved the implementation plan when done in ap md file in the project root → docs folder.
- execute.

- In case if not creating the implementation plan MD file inside the docs folder, please ask it to do so as below
  Your task is to write the implementation plan in the docs folder (which does not exist yet). Your goal is to have 1 complete plan file for the whole project.

- Get the outcome implementation plan and update the context of the project manager( ChatGPT session)

- Ask Claude Code to create agitignore fil for such project.n .gitignore file for such a It must follow the best practices.
