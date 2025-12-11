# User Story to Prompt Template

Break down the provided User Story into logical, incremental tasks suitable for an AI coding assistant. Each task must be clearly defined, testable in isolation, and structured to allow independent implementation, testing, rollback, and deployment without causing breaking changes. Adhere strictly to the following guidelines:

## 1. Incremental and Logical Separation

- Clearly separate tasks by functionality or feature aspect (e.g., presentation layer, business logic, data layer, integration).
- Ensure each task can be independently implemented and tested.
- Group related changes together while maintaining clear boundaries between different concerns.

## 2. Testability and Isolation

### For Presentation Layer Tasks:
- Generate prompts that instruct developers to initially implement presentation components using mock data.
- Clearly state expectations for manual verification of user interactions, emphasizing adjustments before integration with business logic.
- Focus on component behavior, rendering, and user experience validation.

### For Business Logic Tasks:
- Suggest generating implementation prompts using loose Test-Driven Development (TDD) methodology, defining basic tests before writing actual implementation code.
- Emphasize that business logic functionality should be independently testable via unit tests.
- Ensure core functionality is verifiable without external dependencies.

### For Data Layer Tasks:
- Recommend generating tasks that clearly define data structures, schemas, and access patterns.
- Ensure data operations are independently testable with mock or test data sources.
- Validate data integrity and consistency requirements in isolation.

### For Integration Tasks:
- Recommend generating tasks that define integration points and interfaces clearly.
- Suggest testing integration points via appropriate tools (e.g., API testing tools, integration test suites).
- Ensure integration points are explicitly testable via external validation methods.

## 3. Rollback Capability

- Each prompt must explicitly consider rollback scenarios.
- Tasks should minimize dependencies to allow smooth rollback without cascading impacts.
- Design changes to be additive when possible, preserving backward compatibility.
- Document any breaking changes clearly and provide mitigation strategies.

## 4. Semantic Version Control Commits

- After completing each task successfully, clearly instruct the developer to make a semantic commit message to ensure clear, traceable project history.
- Each commit should precisely document the feature, fix, or enhancement implemented.
- Follow conventional commit format (e.g., `feat:`, `fix:`, `refactor:`, `test:`, `docs:`).
- Include scope and clear description of changes in commit messages.

## Usage Guidelines

When applying this template:

1. **Read the User Story carefully** to understand all acceptance criteria and requirements.
2. **Identify natural boundaries** between different aspects of the implementation (presentation, logic, data, integration).
3. **Create discrete tasks** for each boundary, ensuring they can stand alone.
4. **Define success criteria** for each task that can be verified independently.
5. **Order tasks logically** to build upon each other while maintaining independence.
6. **Consider dependencies** but structure tasks to minimize coupling.
7. **Plan for verification** at each stage before moving to dependent tasks.

## Example Task Breakdown Structure

```
User Story: [Original User Story]

Task 1: [Presentation Layer - Component Structure]
- Implement UI components with mock data
- Verify visual behavior and interactions
- Commit: "feat(ui): add [component] with mock data"

Task 2: [Business Logic - Core Functionality]
- Define unit tests for core logic
- Implement business rules and validations
- Verify with test suite
- Commit: "feat(logic): implement [functionality] with tests"

Task 3: [Data Layer - Data Operations]
- Define data structures and access patterns
- Implement data operations with test data
- Verify data integrity
- Commit: "feat(data): add [data operations] with validations"

Task 4: [Integration - Connect Components]
- Connect presentation layer to business logic
- Integrate data layer with business logic
- Verify end-to-end functionality
- Commit: "feat(integration): connect [components] to complete [feature]"
```

## Benefits

- **Clear Progress Tracking**: Each task completion is a milestone.
- **Risk Mitigation**: Issues are isolated to specific tasks, making debugging easier.
- **Flexible Development**: Tasks can be reordered or reassigned as needed.
- **Quality Assurance**: Each task has clear success criteria and verification steps.
- **Maintainable History**: Semantic commits create a readable project timeline.
- **Team Collaboration**: Clear task boundaries facilitate parallel work and code reviews.
