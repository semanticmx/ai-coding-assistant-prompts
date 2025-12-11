# PRD to Backlog Template

Convert the provided Product Requirements Document (PRD) into a complete set of **comprehensive, prioritized user stories** for backlog management, ensuring full coverage of every functional and non-functional requirement described in the PRD.

For **each** PRD requirement, produce a separate user story with the following structure:

**1. User Story** – Write in the format: *As a [type of user], I want [goal or action], so that [reason or benefit].*

**2. Estimated Complexity** – Assign a Fibonacci-based story point estimate (1, 2, 3, 5, 8) reflecting development effort, technical difficulty, and uncertainty.

**3. Acceptance Criteria** – Provide clear, testable, unambiguous conditions for completion, directly traceable to the original PRD requirement.

**4. Performance Targets (SLI/SLO)** – Define measurable Service Level Indicators (SLI) and corresponding Service Level Objectives (SLO) to quantify performance, reliability, scalability, or other quality attributes.

## Final Output Requirements:

* Ensure **100% PRD requirement coverage**, including both functional and non-functional aspects.
* Prioritize user stories based on **business value, user impact, and technical dependencies**, producing a single ordered backlog list ready for integration into a project management tool.
* Use concise, professional language suitable for direct stakeholder review.

## Output Format

Output the stories **in a ready-to-import CSV** format with the following columns:

```csv
Priority,User Story,Estimated Complexity,Acceptance Criteria,SLI/SLO
```

### CSV Format Guidelines:
* **Priority**: Numerical ranking (1, 2, 3, etc.) indicating order of implementation
* **User Story**: Full user story text in the format specified above
* **Estimated Complexity**: Single Fibonacci number (1, 2, 3, 5, or 8)
* **Acceptance Criteria**: Semicolon-separated list of testable conditions
* **SLI/SLO**: Semicolon-separated list of performance metrics and targets

### Example CSV Output:

```csv
Priority,User Story,Estimated Complexity,Acceptance Criteria,SLI/SLO
1,"As a user, I want to log in with my email and password, so that I can access my personalized dashboard.",5,"Login form accepts email and password; Invalid credentials show error message; Successful login redirects to dashboard; Session persists across browser refreshes","Response time SLI: 95% of login requests complete within 2 seconds; Availability SLO: 99.9% uptime for authentication service"
2,"As a system administrator, I want to view user activity logs, so that I can monitor system usage and troubleshoot issues.",3,"Activity log displays user actions with timestamps; Logs are searchable by user and date range; Export functionality available for CSV format","Query performance SLI: 99% of log queries return within 3 seconds; Data retention SLO: Logs retained for minimum 90 days"
```

**Note**: Ensure all CSV fields containing commas or special characters are properly quoted to maintain data integrity across different platforms and tools.
