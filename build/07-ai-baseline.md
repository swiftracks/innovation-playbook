# 07 — AI Baseline

**Purpose**: Build core AI functionality that powers the MVP

**Outcome**: Have a working AI baseline that demonstrates core value

**Audience**: PM / Dev / Both

**Time**: 1-2 weeks

**Prerequisites**: [06 — Setup](06-setup.md)

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Integrate AI API (e.g., OpenAI, Anthropic) into your MVP
2. Build core AI functionality for your use case
3. Implement basic AI features that demonstrate value
4. Handle AI API errors and edge cases
5. Test AI functionality effectively

## Jobs-to-Be-Done

- **When**: I have development environment set up and need to build core AI features
- **I want**: To build AI functionality that demonstrates core value
- **So that**: I can test AI features with real users

## Inputs

- Development environment from [06 — Setup](06-setup.md)
- Understanding of AI requirements from validated hypotheses
- API keys for AI services (e.g., OpenAI)
- Understanding of user needs and use cases

## Activities

### 1. Choose AI Approach

**Select AI Service**:
- **OpenAI**: GPT models, embeddings
- **Anthropic**: Claude models
- **Custom**: Build your own (not recommended for MVP)

**Choose Model**:
- **GPT-4**: Best quality, higher cost
- **GPT-3.5**: Good quality, lower cost
- **Claude**: Alternative option

> 💡 **Tip**: Start with GPT-3.5 for MVP. Upgrade if needed.

### 2. Design AI Integration

**Define AI Features**:
- What will AI do?
- What inputs does it need?
- What outputs does it produce?
- How will it be used?

**Example** (Retrospective Tool):
- **Input**: User feedback from retrospective
- **Output**: AI-generated insights and action items
- **Usage**: User submits feedback → AI generates insights

### 3. Implement AI Integration

**Set Up API Client**:
- Install SDK (e.g., OpenAI Python/Node.js)
- Configure API keys
- Set up error handling
- Implement rate limiting

**Build Core Functionality**:
- Create prompt templates
- Implement API calls
- Handle responses
- Process outputs

**Example Implementation**:
```python
# Pseudocode example
def generate_insights(feedback):
    prompt = f"Analyze this retrospective feedback: {feedback}"
    response = openai.Completion.create(
        model="gpt-3.5-turbo",
        prompt=prompt,
        max_tokens=500
    )
    return response.choices[0].text
```

### 4. Handle Edge Cases

**Error Handling**:
- API failures
- Rate limits
- Invalid inputs
- Timeout handling

**Fallbacks**:
- Default responses
- Retry logic
- User-friendly error messages

### 5. Test AI Functionality

**Testing**:
- Test with real inputs
- Verify outputs are useful
- Test error cases
- Measure performance

**Example Test Cases**:
- Valid input → Useful output
- Invalid input → Error handling
- API failure → Fallback
- Rate limit → Retry logic

## Apply It Now

**Task**: Build AI baseline for your MVP

1. Choose AI service and model
2. Design AI integration for your use case
3. Implement AI API client and core functionality
4. Handle edge cases and errors
5. Test AI functionality with real inputs
6. Document AI integration and usage

**Artifact**: An AI baseline implementation with:
- AI service integration
- Core AI functionality
- Error handling
- Test cases
- Documentation

## Artifacts

You'll create:
- AI API integration
- Core AI functionality
- Error handling logic
- Test cases
- AI documentation

## Worked Example

**Situation**: Building AI baseline for retrospective tool

**AI Approach**:
- Service: OpenAI
- Model: GPT-3.5-turbo
- Use Case: Generate insights from retrospective feedback

**Implementation**:
```python
import openai

def generate_retrospective_insights(feedback):
    prompt = f"""
    Analyze this retrospective feedback and provide:
    1. Key themes
    2. Action items
    3. Recognition points
    
    Feedback: {feedback}
    """
    
    try:
        response = openai.ChatCompletion.create(
            model="gpt-3.5-turbo",
            messages=[
                {"role": "system", "content": "You are a retrospective facilitator."},
                {"role": "user", "content": prompt}
            ],
            max_tokens=500,
            temperature=0.7
        )
        return response.choices[0].message.content
    except Exception as e:
        return f"Error generating insights: {str(e)}"
```

**Testing**:
- Test with sample feedback
- Verify insights are relevant
- Test error cases
- Measure response time

## Checklist

Before proceeding to the next chapter, verify:
- [ ] AI service is integrated
- [ ] Core AI functionality is implemented
- [ ] Error handling is in place
- [ ] AI functionality is tested
- [ ] Documentation is complete

## Self-Assessment

1. **What AI service is good for MVP?**
   - [ ] Custom-built model
   - [ ] OpenAI GPT-3.5 ✓
   - [ ] Complex model fine-tuning

2. **What should you implement?** (Select all)
   - [ ] API client ✓
   - [ ] Core functionality ✓
   - [ ] Error handling ✓
   - [ ] Perfect prompt engineering

3. **What should you test?** (Select all)
   - [ ] Valid inputs ✓
   - [ ] Error cases ✓
   - [ ] Performance ✓
   - [ ] Perfect outputs

## Exit Criteria

You're ready to proceed when:
- [ ] AI service is integrated
- [ ] Core AI functionality is working
- [ ] Error handling is implemented
- [ ] AI functionality is tested
- [ ] You can use AI features in your MVP

## Dependencies & Next Steps

### Prerequisites Completed
- [06 — Setup](06-setup.md) - Development environment

### Next Steps
- Proceed to [08 — Build Features](08-build-features.md) to implement UI based on mockups
- OR proceed to [09 — Deploy](09-deploy.md) to deploy with quality & observability
- These can be done in parallel

### What This Enables

AI baseline enables:
- Core functionality demonstration
- Real user testing
- Learning about AI performance
- Iteration and improvement

---

> 💡 **Tip**: Start simple. You can enhance AI features later.
> 📝 **Note**: Test AI with real inputs early. Don't wait for perfect implementation.

