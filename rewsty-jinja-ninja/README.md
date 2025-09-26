# Rewsty Jinja Ninja

**Specialized Jinja2 templating guidance for Rewst's automation platform.**

## 🎯 Purpose

Rewsty Jinja Ninja is tailored specifically for Rewst's automation platform users, focusing on efficient Jinja2 templating within Rewst's enhanced environment. It guides users on Jinja2 usage, explains limitations, and leverages Rewst's custom filters and enhanced functionality including list/dictionary comprehensions and try-catch capabilities.

## 🔗 Access

**GPT Link**: [Rewsty Jinja Ninja](https://chatgpt.com/g/g-CV7vP7uQ4-rewsty-jinja-ninja)

## 👥 Target Audience

- **Rewst platform users** building automation workflows
- **MSP technicians** creating automated processes and integrations
- **IT professionals** implementing workflow automation solutions
- **Developers** with various programming backgrounds adapting to Jinja2
- **Anyone** working within the Rewst ecosystem who needs Jinja templating help

## ✨ Core Capabilities

### Rewst-Enhanced Jinja2

- **Custom filter support**: Access to Rewst's specialized filter library
- **List/dictionary comprehensions**: Enhanced syntax beyond standard Jinja2
- **Try-catch functionality**: Error handling within Jinja templates
- **Platform-specific patterns**: Best practices for Rewst's workflow environment

### Educational Approach

- **Multi-background support**: Helps users from diverse programming experience levels
- **Best practices emphasis**: Focuses on efficient, maintainable templating patterns
- **Anti-pattern avoidance**: Prevents common inefficiencies and mistakes
- **Practical examples**: Real-world Rewst workflow scenarios

### Reliability Features

- **Documentation verification**: Cross-references solutions against Rewst documentation
- **Error analysis**: Step-by-step breakdown of common Jinja2 errors
- **Compatibility validation**: Ensures recommendations work within Rewst's implementation
- **No speculative suggestions**: Only validated functionality from documented sources

## 🚀 When to Use

### Perfect For:

- **Workflow automation** requiring data transformation and templating
- **Integration patterns** connecting different systems through Rewst
- **Data manipulation** within Rewst automation workflows
- **Template debugging** when Jinja expressions aren't working as expected
- **Performance optimization** of existing Jinja templates
- **Learning Jinja2** specifically within the Rewst context

### Not Ideal For:

- **General Python development** (users can't interact with Python directly)
- **Standard Jinja2 usage** outside of Rewst platform
- **Complex algorithmic logic** better suited for other tools
- **Frontend templating** in web development contexts

## 💡 Usage Tips

### Understanding Rewst Context

1. **No Python access**: Remember you're working within Rewst's workflow environment
2. **Enhanced features**: Leverage comprehensions and try-catch beyond standard Jinja2
3. **Filter validation**: All suggestions use documented Rewst filters only
4. **Workflow integration**: Consider how templates fit into broader automation flows

### Example Prompts

```
"I need to transform a list of users from an API response into a
formatted list for email notification. The API returns user objects
with name, email, and department fields."

"How can I safely handle API responses that might be missing
expected fields? I want to avoid workflow failures when data
structure varies."

"I have a complex nested JSON response and need to extract
specific values for different workflow branches. What's the
most efficient approach in Rewst?"
```

### Getting Best Results

- **Show your data structure**: Include examples of input data
- **Explain your goal**: What output format you need
- **Mention error messages**: Include any Jinja errors you're encountering
- **Provide context**: How this fits into your broader workflow

## 📊 Enhanced Jinja2 Features in Rewst

### List/Dictionary Comprehensions

Standard approach:

```jinja2
{% set user_ids = [] %}
{% for user in CTX.list_of_users %}
  {% set _ = user_ids.append(user.id) %}
{% endfor %}
{{ user_ids }}
```

Enhanced Rewst approach:

```jinja2
{{ [user.id for user in CTX.list_of_users] }}
```

### Try-Catch Functionality

```jinja2
{% try %}
  {{ potentially_missing_field.value }}
{% catch %}
  "Default value"
{% endtry %}
```

### Custom Filters

Access to Rewst's specialized filter library for:

- **Data transformation**: Custom formatting and conversion
- **API response handling**: Specialized JSON and XML processing
- **Integration patterns**: Platform-specific data manipulation

## ⚡ Best Practices

### Efficiency Guidelines

1. **Prefer comprehensions**: More efficient than manual loops for simple transformations
2. **Use try-catch**: Graceful error handling prevents workflow failures
3. **Leverage custom filters**: Take advantage of Rewst's specialized functionality
4. **Validate data structures**: Check for expected fields before processing

### Common Patterns

- **Safe data access**: Always handle potential missing keys/fields
- **Batch processing**: Efficient handling of lists and collections
- **Conditional logic**: Clean branching based on data conditions
- **Error recovery**: Graceful fallbacks when data doesn't match expectations

### Anti-Patterns to Avoid

- **Hardcoded values**: Use variables and context data instead
- **Complex nested loops**: Consider comprehensions or filter chains
- **Unhandled errors**: Always plan for data variations
- **Python-specific assumptions**: Remember Jinja2 limitations within Rewst

## 🔍 Error Analysis Framework

### Error Breakdown Process

1. **Error type identification**: Undefined variable, incompatible data type, etc.
2. **Context analysis**: What data was expected vs what was received
3. **Solution space**: Available filters, logic constructs, patterns that work
4. **Documentation verification**: Confirm all recommendations are validated

### Common Error Scenarios

- **Undefined variable errors**: When context data doesn't match expectations
- **Type errors**: Applying wrong operations to data types
- **Filter errors**: Using incorrect or non-existent filters
- **Syntax errors**: Malformed Jinja2 expressions

## 💭 Knowledge Sources

### Validated References

- **Rewst documentation**: Complete platform documentation for context and patterns
- **Custom filters library**: Full filter reference with usage examples
- **Jinja comprehensions**: Enhanced syntax documentation and implementation details
- **Try-catch functionality**: Error handling patterns and best practices

### Reliability Commitment

- **No assumptions**: Every recommendation verified against documentation
- **Systematic validation**: Cross-reference solutions with multiple sources
- **Explicit uncertainty**: Clear statements when features aren't documented
- **Practical focus**: Solutions that work in real Rewst environments

## 🎯 Example Use Cases

### Data Transformation

```jinja2
# Transform API user list to email-friendly format
{{ [user.email for user in users if user.active and user.department == 'IT'] }}
```

### Safe Data Access

```jinja2
# Handle potentially missing API fields
{% try %}
  {{ api_response.data.users | length }}
{% catch %}
  0
{% endtry %}
```

### Conditional Processing

```jinja2
# Different handling based on data type
{% if incident.priority == 'high' %}
  {{ incident | format_urgent_notification }}
{% else %}
  {{ incident | format_standard_notification }}
{% endif %}
```

---

_For technical instructions and GPT configuration details, see [`instructions.md`](instructions.md)_
