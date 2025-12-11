# AI Coding Assistant Prompts

A collection of prompt templates designed to streamline the software development workflow from Product Requirements Documents (PRD) to implementation using AI coding assistants.

## Overview

This repository provides a structured approach to transforming business requirements into actionable development tasks that can be efficiently executed with AI coding assistants. The workflow ensures clarity, consistency, and comprehensive documentation throughout the development process.

## Workflow

The prompts follow a sequential workflow that breaks down product development into manageable stages:

```
PRD Prompt Template
        ↓
PRD to Backlog Template
        ↓
User Story to Prompt Template
        ↓
AI Coding Assistant Implementation
```

### Stage 1: PRD Creation (PRD Prompt Template)

**Purpose:** Generate a comprehensive Product Requirements Document from high-level product ideas or features.

**How to use:**
1. Start with your product idea, feature request, or business requirement
2. Use the **PRD Prompt Template** to guide the AI in creating a detailed PRD
3. The template helps structure:
   - Problem statement and goals
   - User personas and use cases
   - Functional and non-functional requirements
   - Success metrics and acceptance criteria
   - Technical considerations and constraints

**Example prompt:**
```
Using the PRD Prompt Template, create a PRD for [your feature/product idea].
Include target users, key functionalities, and technical requirements.
```

### Stage 2: Backlog Generation (PRD to Backlog Template)

**Purpose:** Transform the PRD into a prioritized backlog of user stories and tasks.

**How to use:**
1. Take the completed PRD from Stage 1
2. Apply the **PRD to Backlog Template** to break down requirements into:
   - Epic-level stories
   - Detailed user stories with acceptance criteria
   - Technical tasks and dependencies
   - Priority rankings
3. The output should be a structured backlog ready for sprint planning

**Example prompt:**
```
Using the PRD to Backlog Template, convert this PRD into a prioritized backlog:
[Paste your PRD here]

Focus on breaking down features into implementable user stories.
```

### Stage 3: Task Generation (User Story to Prompt Template)

**Purpose:** Convert user stories into specific, actionable prompts for AI coding assistants.

**How to use:**
1. Select a user story from your backlog
2. Use the **User Story to Prompt Template** to create detailed implementation prompts
3. Each prompt should include:
   - Clear context and objectives
   - Specific acceptance criteria
   - Technical constraints and requirements
   - File/component locations
   - Testing requirements

**Example prompt:**
```
Using the User Story to Prompt Template, create implementation prompts for:
User Story: [Story description]
Acceptance Criteria: [Criteria list]

Generate prompts suitable for an AI coding assistant.
```

### Stage 4: Implementation with AI Coding Assistant

**Purpose:** Execute the development tasks using your AI coding assistant.

**How to use:**
1. Take the prompts generated in Stage 3
2. Feed them to your AI coding assistant (e.g., GitHub Copilot, Cursor, Claude, etc.)
3. The AI assistant will:
   - Implement the required functionality
   - Create or modify code files
   - Write tests
   - Update documentation
4. Review, test, and iterate on the AI-generated code

**Example:**
```
[Paste the detailed prompt from Stage 3 to your AI coding assistant]

The assistant should have all the context needed to implement the feature.
```

## Best Practices

### For PRD Creation
- Be specific about user needs and pain points
- Include measurable success criteria
- Document technical constraints early
- Consider scalability and maintainability

### For Backlog Generation
- Keep user stories small and independently deliverable
- Define clear acceptance criteria for each story
- Identify and document dependencies
- Prioritize based on value and risk

### For Prompt Creation
- Provide sufficient context about the codebase
- Be explicit about coding standards and patterns
- Include examples when possible
- Specify testing requirements

### For AI Implementation
- Review generated code for security and quality
- Run tests after each implementation
- Iterate on prompts if results don't meet expectations
- Document any deviations from the original plan

## Tips for Success

1. **Start Small**: Begin with a small feature to familiarize yourself with the workflow
2. **Iterate**: Don't expect perfection on the first pass - refine your prompts based on results
3. **Context is Key**: Provide as much relevant context as possible at each stage
4. **Review Carefully**: Always review AI-generated content, especially code
5. **Maintain Consistency**: Use the templates consistently across projects for better results
6. **Version Control**: Keep track of prompt versions that work well for future reference

## Example Workflow

Here's a complete example workflow:

### 1. Start with an Idea
"We need a user authentication system with email and password login."

### 2. Create PRD
Use PRD Prompt Template to generate a comprehensive PRD covering:
- Authentication requirements
- Security considerations
- User flows
- API specifications

### 3. Generate Backlog
Use PRD to Backlog Template to create stories like:
- "As a user, I can register with email and password"
- "As a user, I can log in with my credentials"
- "As a user, I can reset my forgotten password"

### 4. Create Implementation Prompts
Use User Story to Prompt Template for each story:
- "Implement user registration endpoint with email validation, password hashing, and database storage..."

### 5. Implement with AI
Feed prompts to your AI coding assistant and build the feature iteratively.

## Contributing

This repository is designed to help teams leverage AI coding assistants effectively. As you use these templates, consider contributing improvements or new templates that enhance the workflow.

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## Getting Started

1. Review this README thoroughly
2. Prepare your product idea or feature request
3. Follow the workflow from Stage 1 through Stage 4
4. Iterate and refine based on results
5. Share feedback and improvements with the community

Happy building with AI! 🚀
