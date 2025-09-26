# Socratic Dev Critique

**Systematic design review and mental model application for frontend, architecture, and systems development.**

## 🎯 Purpose

Socratic Dev Critique is a design reviewer and mental model translator that operationalizes developer mental models as semantic shorthands. It automatically applies the Socratic Reflection Protocol (SRP) to evaluate code, architecture, and design decisions using established mental models from industry experts, focusing on systemic safety and maintainability.

## 🔗 Access

**GPT Link**: [Socratic Dev Critique](https://chatgpt.com/g/g-685624068aec8191b44558cf5655599e-socratic-dev-critique)

## 👥 Target Audience

- **Frontend developers** building React applications and component systems
- **System architects** designing scalable, maintainable applications
- **Team leads** conducting code reviews and architectural reviews
- **Engineers** who want to apply industry best practices systematically
- **Anyone** building software that needs to scale and be maintainable by teams

## ✨ Core Mental Model Stack

### 14 Mental Models for React Systems Engineering

#### 1. **MARCOTTE** - Layout & Responsive Discipline

- Mobile-first, fluid grids
- Flex/Grid dominance
- Accessibility from first render
- Context-aware adaptive components

#### 2. **FROST** - Component Hierarchy System

- Atoms → Molecules → Organisms → Templates → Pages
- Reusable design system primitives
- Separation of presentational vs container logic

#### 3. **ABRAMOV** - State Management Discipline

- Predictable state flows
- Controlled components by default
- Single sources of truth per feature boundary
- State machines/reducers for complex flows

#### 4. **KRUG** - User Experience Clarity

- Users shouldn't have to think
- Obvious affordances
- Minimal clicks to intent
- Consistent visual language

#### 5. **RAUCH** - Performance Architecture

- Server-first rendering (SSR, edge rendering)
- Minimal client hydration
- Avoid client bloat and unnecessary re-renders
- Intelligent lazy loading

#### 6. **FLORENCE** - Complex Flow Integrity

- Clear async ownership boundaries
- Stable re-renders during interactive flows
- Safe nested state orchestration
- Prevention of ghost states during optimistic updates

#### 7. **SPOLSKY** - Behavioral Contracts Discipline

- Explicit edge case definitions
- Defensive UI states (loading, error, null, success)
- No ambiguous or silent failure states
- Documented prop types/contracts

#### 8. **MCILROY** - Data Input Sanitation

- Validate every inbound data shape
- Strict sanitization of external API responses
- Schema validation (Zod, Yup, io-ts)
- Never assume external trust

#### 9. **BERGLUND** - Secure Defaults Discipline

- Least privilege everywhere
- No implicit data access privileges
- CORS, CSRF, OAuth, input sanitation as default
- Secure secrets management and token flows

#### 10. **SHAPIRO** - Async State Safety

- Clear ownership tied to component boundaries
- Cancellation, retry, timeout handling
- Graceful fallback UIs during async disruptions
- Prevention of race condition vulnerabilities

#### 11. **TUFTE** - Data-Dense UI Excellence

- High data-to-ink ratio
- Avoid meaningless dashboards or vanity metrics
- Small multiples and sparklines where needed
- Drilldown pathways without clutter

#### 12. **REINERTSEN** - Flow Efficiency Thinking

- Minimize blocking UI states
- Avoid coupled dependencies in load chains
- Progressive disclosure of data
- Keep Work-In-Progress (WIP) low

#### 13. **LE BLANC** - Developer Cognitive Load Reduction

- Predictable naming conventions
- Standardized file structures
- Explicit prop contracts
- TypeScript for exhaustive design-time safety

#### 14. **DORSEY** - Operational Resilience & Observability

- Full instrumentation of live state
- Structured logs, traces, metrics
- Feature flag safety releases
- Incident-ready design (circuit breakers, fallbacks)

## 🚀 When to Use

### Perfect For:

- **Code reviews** requiring systematic evaluation
- **Architecture decisions** with long-term implications
- **Performance optimization** of React applications
- **System design** for scalable frontend applications
- **Team education** on industry best practices
- **Pre-production safety checks** before deployment

### Not Ideal For:

- **Simple bug fixes** with obvious solutions
- **Quick prototyping** where speed trumps structure
- **Non-React frontend frameworks** (though principles may apply)
- **Backend system design** outside frontend concerns

## 💡 Usage Tips

### Input Guidelines

1. **Share your code**: Include actual implementation details
2. **Provide context**: Team size, performance requirements, constraints
3. **Ask specific questions**: "Is this component structure maintainable?"
4. **Request mental model application**: "Apply ABRAMOV principles to this state logic"

### Example Prompts

```
"Review this React component for maintainability and performance.
Apply relevant mental models and identify potential issues."

"I'm designing a data-heavy dashboard component. Apply TUFTE
and REINERTSEN principles to evaluate the approach."

"This form component is getting complex. Use ABRAMOV and FROST
mental models to suggest improvements."
```

### Getting Best Results

- **Include complete code context**: Don't just show snippets
- **Mention your concerns**: What specifically worries you about the implementation?
- **Ask for specific mental models**: Reference experts by name (MARCOTTE, ABRAMOV, etc.)
- **Request "If I Left Tomorrow" analysis**: How maintainable is this for new team members?

## 📊 Socratic Reflection Protocol (SRP)

Applied automatically to every review:

### 1. Boundaries of Responsibility

- Which component owns this state?
- Where are async boundaries?
- Are responsibilities clearly separated?

### 2. State Ownership Validation

- Is state managed at the right level?
- Are there conflicting sources of truth?
- How does state flow through the system?

### 3. Scaling Safety

- Will this perform at 10x data load?
- Can it handle 100x concurrent users?
- What breaks first under pressure?

### 4. Data Shape & Contracts

- Are inputs/outputs schema validated?
- Are prop contracts well-defined?
- How do we handle unexpected data?

### 5. Cognitive Load Audit

- Is this system predictable for new developers?
- Are patterns consistent across the codebase?
- What assumptions require tribal knowledge?

### 6. The "If I Left Tomorrow" Test

- Could a new developer safely extend this feature?
- Is the reasoning documented and discoverable?
- What would break if original author left?

## ⚡ Response Format

### Builder Instructions First

Every response begins with a concise, actionable list:

```
BUILDER INSTRUCTIONS:
1. Extract user list logic to custom hook (ABRAMOV pattern)
2. Add error boundaries around async components (SPOLSKY pattern)
3. Implement loading states for all data fetches (KRUG pattern)
4. Add TypeScript interfaces for all props (LE BLANC pattern)
5. Consider server-side rendering for performance (RAUCH pattern)
```

### Detailed Analysis Second

Following the builder instructions:

- **Mental model application**: Which patterns apply and why
- **Specific improvements**: Code-level recommendations
- **Trade-off analysis**: Costs and benefits of suggested changes
- **Risk assessment**: What could go wrong with current approach

## 🎯 Expert Mental Model Invocation

### Direct Expert Application

When you invoke an expert name:

- **MARCOTTE**: Full responsive and accessibility review
- **ABRAMOV**: Complete state management analysis
- **FROST**: Component hierarchy and design system evaluation
- **KRUG**: User experience and usability assessment

### Cross-Domain Analysis

Most real systems require multiple mental models:

- **ABRAMOV + FLORENCE**: Complex state + async flow management
- **FROST + LE BLANC**: Component design + developer experience
- **RAUCH + SHAPIRO**: Performance + async safety

## 🔍 Example Review Output

**Input**: React component with complex form state and API calls

**Response**:

```
BUILDER INSTRUCTIONS:
1. Replace useState with useReducer for form state (ABRAMOV)
2. Add error boundaries for API failure handling (SPOLSKY)
3. Implement proper loading states (KRUG)
4. Extract reusable form components (FROST)
5. Add input validation schema (MCILROY)

JUSTIFICATION (Optional):

ABRAMOV Analysis - State Management:
Your current useState approach creates multiple state updates that can race...

SPOLSKY Analysis - Behavioral Contracts:
Missing error states mean users see blank screens when APIs fail...

KRUG Analysis - UX Clarity:
No loading indicators leave users uncertain about system status...
```

## 💭 Philosophy

**Curious, exploratory, rigorous**—Socratic Dev Critique:

- **Questions before judgments**: Invites reflection and reasoning
- **Systematic safety**: Prioritizes long-term maintainability
- **Fresh perspective**: Evaluates as though new engineer is reading
- **No oral history assumptions**: Everything should be discoverable from code

The goal is uncovering hidden coupling, brittle assumptions, and cognitive load traps before they become production problems.

---

_For technical instructions and GPT configuration details, see [`instructions.md`](instructions.md)_
