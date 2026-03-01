  ---
  name: Design                                                                                                                                                  
  description: "Use this skill when the task is ambiguous or if explicitly requested."                                                                                                         
  metadata:                                                                                                                                                              
    short-description: Design for clarifying ambiguous problems.                                                                                                                   
  ---                                                                                                                                                                    
                                                                                                                                                                         
  ## Purpose                                                                                                                                                             
  Some engineering problems start as ambiguous ideas and need multiple iterations to clarify 
  what needs to  be implemented. Such problems also deal with multiple design decisions and
  tradeoffs. It is important to make all these decisions before writing any code.
                                                                                                                                                                         
  ## Non-negotiables
  1. DO NOT EDIT CODE
  2. Serena first: Start by activating the Serena project (if the Serena tools exist in the environment). If activation fails for reasons outside your control, inform the user.
  3. Investigate before changing anything: Understand the current state (application state, execution results) before proposing edits.
  4. Understand the problem as much as possible before proposing solutions. Ask clarifying questions.
  5. Write the design in a file DESIGN.md. If DESIGN.md exists, ask for confirmation before overwriting and keep a backup copy when overwriting. Use the mandated structure (below).
  6. Use up-to-date docs: When you rely on an API/package/technology detail, use Kindly Web Search (if available) to confirm signatures, version behavior, breaking changes, and deprecations.
  7. If the project requires deep understanding of a complex new techology beyond a few web searches, ask the user to run deep research.
                                                                                                                                                                         
  ## DESIGN.md Structure (Mandated)
  Write/overwrite DESIGN.md in the target repository root with:
  1. **Context**: Describe current state of the relevant parts of the system, if possible add links to
  serena docs or generally the project documentation.
  2. **Problem**: Describe the problem the user posed with all the details and clarifications.
  3. **List of subproblems with solutions**: For each subproblem include short description, all 
  alternative solutions considerred with pros/cons analysis and the preferred solution.
                                                                                                                                                                         
  ## Workflow                                                                                                                                                            
  ### 1) Understand the problem                                                                                                                                                     
  - Deeply understand what the user is trying to build
  - Ask multiple clarifying questions
  - Ask Lad MCP Server to review problem statement to make sure it is clear. Incorporate the feedback. Continue the rounds of review with Lad until it stops providing useful feedback
  - Ask user to confirm the summarized detailed problem description
  - Write the detailed description of the problem in the Problem section in DESIGN.md
                                                                                                                                                                         
  ### 2) Understand the context                                                                                                                                                            
  - Summarize the parts of the project relevant to the problem. Focus on components and architecture
  - Link relevant pieces of code and documentation
  - Use Kindly Web Search to look for additional context 
  - If the required context is beyond what can be clarified by a few searches (ex. user requested to use a completely new technology, or the problem seems to only be described in scientific papers) ask the user to provide more context through deep research.
  - Ask Lad MCP Server to review the context and suggest additional questions to resolve.Incorporate the feedback. Continue the rounds of review with Lad until it stops providing useful feedbackю
  - Write all the pieces of context in DESIGN.md

  ### 3) Split problem into subproblems                                                                                                                                                       
  - Use context to guide the split                                                                                                                                           
  - Ask Lad MCP Server to review the proposed splitю Incorporate the feedback. Continue the rounds of review with Lad until it stops providing useful feedback
  - Ask the user to confirm the split
                                                                                                                                                                         
  ### 4) Solve the subproblems one by one                                                                                                                                                        
  - For each subproblem suggest alternative solutions
  - Analyze pros and cons of the solution
  - Ask Lad MCP Server to review the reasoningю Incorporate the feedback. Continue the rounds of review with Lad until it stops providing useful feedback.
  - Select the best of the proposed solutions
  - Ask the user to review the alternatives and confirm the preferred solution.
  - Write the section to DESIGN.md

  ### Review the design
  - Review the design with Lad MCP
  - If Lad suggests new subproblems to consider follow the subproblem solving instructions.
  - Incorporate the feedback. Continue the rounds of review with Lad until it stops providing useful feedback.
