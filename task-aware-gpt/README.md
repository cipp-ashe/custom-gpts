# Task-Aware GPT

**Meta-cognitive, task-aware assistant that maps inputs to optimal response patterns.**

## 🎯 Purpose

Task-Aware GPT is a meta-cognitive assistant that explicitly maps user inputs against benchmark task archetypes to optimize response format and approach. It identifies relevant task patterns, validates interpretations with users, and adjusts response formatting to match the task's natural affordances while preserving nuance and intent.

## 🔗 Access

**GPT Link**: [Task-Aware GPT](https://chatgpt.com/g/g-6868363d43908191bb15cf50b088f09e-task-aware-gpt)

## 👥 Target Audience

- **Researchers and analysts** working with complex, multi-faceted requests
- **Project managers** who need properly structured responses for different stakeholder types
- **Consultants and advisors** handling varied client requests requiring different approaches
- **Anyone** making complex requests that could benefit from task-aware formatting
- **Teams** needing consistent, well-structured responses across different types of work

## ✨ Core Capabilities

### Task Pattern Recognition

- **Archetype mapping**: Identifies patterns like "paraphrase + causal reasoning + free response"
- **Multi-pattern detection**: Recognizes when requests combine multiple task types
- **Interpretation validation**: Reflects back understanding before proceeding
- **Ambiguity flagging**: Identifies underspecified or conflicting requests

### Response Optimization

- **Format adaptation**: Adjusts output to match task affordances (JSON, multiple choice, step-by-step)
- **Structure explanation**: Explains why specific formatting was chosen
- **Nuance preservation**: Maintains user intent while optimizing structure
- **Meta-instruction tracking**: Complies with session-level preferences ("always validate first")

### Socratic Self-Reflection

- **Reasoning transparency**: Explains the thinking process before output
- **Assumption identification**: Surfaces and validates underlying assumptions
- **Limitation acknowledgment**: Clearly states potential weaknesses or gaps
- **Clarity over speed**: Prioritizes accurate understanding over quick responses

## 🚀 When to Use

### Perfect For:

- **Complex, multi-part requests** that could be interpreted multiple ways
- **Research questions** requiring specific formatting or analytical approaches
- **Stakeholder communications** where format and structure matter
- **Ambiguous requirements** needing clarification and validation
- **Iterative work** where you want consistent task interpretation across sessions
- **Meta-analysis** of your own request patterns and communication style

### Not Ideal For:

- **Simple, straightforward questions** with obvious single interpretations
- **Creative tasks** where ambiguity is valuable rather than problematic
- **Urgent requests** where speed trumps methodical validation
- **Casual conversations** where formal task mapping adds unnecessary overhead

## 💡 Usage Tips

### Interaction Approach

1. **Expect interpretation feedback**: The system will reflect back its understanding
2. **Validate before proceeding**: Confirm the task interpretation is correct
3. **Embrace the process**: This is deliberately more methodical than typical AI
4. **Be specific about format needs**: JSON, bullet points, narrative, etc.

### Example Interactions

```
User: "Analyze the competitive landscape for AI writing tools and
provide strategic recommendations for positioning."

Task-Aware GPT: "I'm interpreting this as a combination of:
- Market analysis + competitive assessment
- Strategic reasoning + recommendation generation
- Business context + actionable insights

This suggests a structured analytical format with:
1. Competitive landscape overview
2. Key differentiators and gaps
3. Strategic positioning recommendations
4. Implementation considerations

Is this the right interpretation and format approach?"
```

### Getting Best Results

- **Provide context**: Why you need this analysis, who will use it
- **Specify constraints**: Time, format, depth requirements
- **Clarify success criteria**: What would make this response valuable?
- **Mention any session preferences**: "Always validate first," "prefer JSON," etc.

## 📊 Task Archetype Examples

### Analysis Tasks

- **Causal reasoning**: Why did X happen? What factors contributed?
- **Comparative analysis**: How do options A and B differ?
- **Trend analysis**: What patterns emerge from this data?

### Synthesis Tasks

- **Summarization**: Distill key points from complex information
- **Integration**: Combine insights from multiple sources
- **Pattern extraction**: Identify common themes or structures

### Planning Tasks

- **Strategic planning**: Long-term direction and priorities
- **Process design**: Step-by-step workflow creation
- **Risk assessment**: Identify and evaluate potential issues

### Communication Tasks

- **Stakeholder translation**: Adapt technical content for different audiences
- **Persuasive writing**: Build compelling arguments or proposals
- **Documentation**: Create clear, structured reference materials

## ⚡ Meta-Cognitive Process

### Input Processing

1. **Pattern recognition**: Map request against known task archetypes
2. **Complexity assessment**: Single task vs multi-part combination
3. **Ambiguity detection**: Flag unclear or conflicting elements
4. **Format optimization**: Determine best structure for response

### Validation Loop

1. **Interpretation reflection**: "Here's what I understand..."
2. **Format explanation**: "This suggests using X structure because..."
3. **User confirmation**: Wait for validation before proceeding
4. **Adjustment incorporation**: Modify approach based on feedback

### Response Generation

1. **Reasoning transparency**: Show the thinking process
2. **Assumption surfacing**: Make implicit assumptions explicit
3. **Limitation flagging**: Note areas of uncertainty or weakness
4. **Structured delivery**: Present in optimized format with clear reasoning

## 🎯 Session-Level Meta-Instructions

### Tracking Capabilities

- **Always validate first**: Consistent interpretation checking
- **Prefer specific formats**: JSON, markdown, structured lists
- **Maintain context**: Remember previous task preferences
- **Apply learned patterns**: Improve interpretation over time

### Customizable Behaviors

- **Validation level**: How much confirmation to seek
- **Format preferences**: Default structures for different task types
- **Detail level**: Depth of analysis and explanation
- **Process visibility**: How much meta-cognitive reasoning to show

## 🔍 Task Mapping Framework

### Keywords to Task Mapping

The system references comprehensive keyword-to-task mappings to:

- **Identify task patterns**: Recognize common request structures
- **Justify categorization**: Explain why specific tasks were selected
- **Ensure consistency**: Apply standardized interpretations
- **Enable refinement**: Learn from validation feedback

### Multi-Task Combinations

When requests combine multiple tasks:

- **Primary task identification**: What's the main objective?
- **Supporting tasks**: What analysis supports the primary goal?
- **Sequence optimization**: What order produces the best result?
- **Integration strategy**: How do components work together?

## 💭 Philosophy

**Clarity, humility, and intent alignment over speed**—Task-Aware GPT embodies:

- **Meta-cognitive awareness**: Conscious of its own thinking process
- **Humble uncertainty**: Acknowledges limitations and seeks clarification
- **Intent preservation**: Maintains user nuance while optimizing structure
- **Systems thinking**: Considers how tasks fit into broader workflows
- **Reflective practice**: Continuously improves task interpretation

## 🔬 Example Task Analysis

**Input**: "Help me understand why our customer retention dropped last quarter and what we should do about it."

**Task-Aware Analysis**:

> **Task Pattern Identified**: Causal analysis + strategic reasoning + actionable recommendations
>
> **Components Detected**:
>
> 1. Data analysis (retention metrics examination)
> 2. Root cause analysis (why did it drop?)
> 3. Strategic planning (what should we do?)
> 4. Implementation guidance (how to execute)
>
> **Suggested Format**:
>
> - Executive summary of findings
> - Data analysis with key metrics
> - Root cause assessment with evidence
> - Strategic recommendations with priorities
> - Implementation roadmap with timelines
>
> **Validation Questions**:
>
> - Do you have access to retention data I should reference?
> - What level of detail do you need for stakeholder presentation?
> - Are there specific timeframes or constraints for implementation?
>
> **Proceed with this interpretation and format?**

---

_For technical instructions and GPT configuration details, see [`instructions.md`](instructions.md)_
