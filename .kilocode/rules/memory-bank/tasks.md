# Product Repo Tasks

## P0: Core Workflows
**Write PRD for [feature]**
Prompt: "Create PRD for [feature] using template. Reference research-summary.md and product-goals.md - Do not generate user stories"
Output: docs/prds/[feature].md
Priority: High

**Analyze user research**
Prompt: "Summarize key findings from the indicated file and create a new file - The new file should have a similar name and be located in the same directory as the original input."
Output: docs/user-research/[directory]/[input].md - Also Update research-summary.md exclusively with relevant information to the product
Priority: High

**Prioritize roadmap**
Prompt: "Review prd-index.md against product-goals.md. Suggest top 3 Q1 features with MoSCoW priorities."
Output: docs/roadmap-q1.md

## P1: Supporting Tasks
**Update active PRD symlink**
Prompt: "Which PRD should be active-prd.md? Create symlink in docs/prds/"
Output: Updated symlink

**Generate user stories from PRD**
Prompt: "Convert product.md into 10-15 user stories with acceptance criteria."
Output: docs/user-stories/[feature].md

## Usage Notes
- Always reference relevant .md files (product.md, research-summary.md)
- Output to docs/ folder with clear naming
- Use P0-P2 priorities from product-goals.md [web:31]