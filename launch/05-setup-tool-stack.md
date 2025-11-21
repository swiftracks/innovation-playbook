# 05 — Setup Tool Stack

**Purpose**: Set up standard tool stack for launch operations

**Outcome**: Have complete tool stack set up for website, analytics, social monitoring, and content development with all tools integrated to feed data into Swift CNS experiments

**Audience**: PM / Dev / Both

**Time**: 2-3 days

**Prerequisites**: [04 — Build Website V1](04-build-website-v1.md) - Website built

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Set up website stack (standard recommendation)
2. Set up analytics stack (product analytics)
3. Set up social monitoring stack
4. Set up content development stack (AI tools + human process)
5. Develop base context for AI prompting
6. Create automated content generation workflows
7. Integrate all tools to feed data into Swift CNS experiments

## Jobs-to-Be-Done

- **When**: I have website V1 built and need tools for launch operations
- **I want**: To set up a complete tool stack for tracking and operations
- **So that**: I can track performance, monitor channels, create content, and feed all data into Swift CNS experiments

## Inputs

- Website V1 from [04 — Build Website V1](04-build-website-v1.md)
- Understanding of what to track
- Budget for tools
- Swift CNS account for experiment tracking

## Activities

### 1. Set Up Website Stack

**Standard Website Stack Recommendation**:

**Option 1: Webflow** (Recommended for most)
- **Pros**: Visual builder, good for non-developers, hosting included
- **Cons**: Learning curve, monthly cost
- **Best For**: Teams wanting visual control without coding
- **Cost**: $12-35/month

**Option 2: Framer** (Recommended for modern design)
- **Pros**: Modern design tools, good animations, hosting included
- **Cons**: Learning curve, monthly cost
- **Best For**: Design-focused teams
- **Cost**: $5-20/month

**Option 3: Custom** (For developers)
- **Pros**: Full control, no monthly cost
- **Cons**: Requires development, hosting setup
- **Best For**: Teams with development resources
- **Cost**: Hosting only ($5-20/month)

**Website Stack Setup**:
1. Choose platform (Webflow/Framer/Custom)
2. Set up account
3. Build website V1 (or migrate existing)
4. Configure domain
5. Set up SSL (HTTPS)
6. Test website

**Integration Requirements**:
- Analytics integration (see Analytics Stack)
- Form handling (signup, contact)
- UTM parameter tracking
- Error tracking

**Document in Swift CNS**:
- Create website stack documentation
- Document integrations
- Plan website experiments

### 2. Set Up Analytics Stack

**Product Analytics Stack Recommendation**:

**Option 1: Mixpanel** (Recommended)
- **Pros**: Product analytics focused, good segmentation, free tier
- **Cons**: Can be complex, pricing scales
- **Best For**: Product analytics and user behavior
- **Cost**: Free up to 20M events/month, then $25+/month

**Option 2: Amplitude** (Alternative)
- **Pros**: Product analytics focused, good free tier
- **Cons**: Can be complex
- **Best For**: Product analytics and user behavior
- **Cost**: Free up to 10M events/month, then $25+/month

**Option 3: PostHog** (Open source alternative)
- **Pros**: Open source, self-hostable, good features
- **Cons**: Requires setup, self-hosting complexity
- **Best For**: Teams wanting open source
- **Cost**: Free (self-hosted) or $20+/month (cloud)

**Analytics Setup**:
1. Choose analytics tool
2. Create account
3. Install SDK (frontend + backend if needed)
4. Set up event tracking
5. Create dashboards
6. Set up alerts

**Essential Events to Track**:
- User signup
- User login
- Core feature usage
- Journey completion
- Errors and issues
- Channel attribution (UTM parameters)

**Analytics Integration**:
- Website integration (track page views, CTAs)
- Product integration (track feature usage)
- Channel integration (track traffic sources)
- Swift CNS integration (feed data to experiments)

**Document in Swift CNS**:
- Create analytics setup documentation
- Document event tracking
- Create analytics experiment plans

### 3. Set Up Social Monitoring Stack

**Social Monitoring Stack Recommendation**:

**Social Media Management**:

**Option 1: Buffer** (Recommended)
- **Pros**: Simple, good free tier, multiple platforms
- **Cons**: Limited features on free tier
- **Best For**: Simple social media management
- **Cost**: Free (3 accounts), $6+/month (more accounts)

**Option 2: Hootsuite** (Alternative)
- **Pros**: Comprehensive, good analytics
- **Cons**: More complex, higher cost
- **Best For**: Teams needing comprehensive management
- **Cost**: $99+/month

**Social Monitoring Setup**:
1. Choose social media management tool
2. Connect social accounts (LinkedIn, Twitter/X, etc.)
3. Set up posting schedule
4. Set up monitoring (mentions, keywords)
5. Set up analytics tracking

**Monitoring Setup**:
- **Mentions**: Track brand mentions
- **Keywords**: Track relevant keywords
- **Competitors**: Monitor competitor activity
- **ICP**: Monitor ICP discussions
- **Channels**: Monitor warm channels

**Social Integration**:
- Channel integration (track social performance)
- Analytics integration (track social traffic)
- Swift CNS integration (feed social data to experiments)

**Document in Swift CNS**:
- Create social monitoring setup documentation
- Document monitoring keywords
- Create social experiment plans

### 4. Set Up Content Development Stack

**Content Development Stack**:

**AI Tools**:

**Option 1: ChatGPT** (Recommended)
- **Pros**: Good for content creation, versatile
- **Cons**: Requires good prompts, subscription for best features
- **Best For**: General content creation
- **Cost**: Free (limited), $20/month (GPT-4)

**Option 2: Claude** (Alternative)
- **Pros**: Good for long-form content, good reasoning
- **Cons**: Requires good prompts
- **Best For**: Long-form content, analysis
- **Cost**: Free (limited), $20/month (Claude Pro)

**AI Content Process**:
1. Develop base context (ICP, messaging, product)
2. Create prompt templates
3. Generate content variations
4. Human review and edit
5. Publish and track

**Base Context Development**:

**What to Include in Base Context**:
- ICP framework (from chapter 01)
- Messaging strategy (from chapter 02)
- Product features and benefits
- Brand voice and tone
- Content guidelines

**Example Base Context**:
```
ICP: Engineering Managers at SaaS companies (50-500 employees)
Messaging: "Turn retrospectives into action in 30 minutes"
Key Benefits: 50% faster retrospectives, actionable insights, clear action items
Brand Voice: Professional, helpful, direct
Content Guidelines: Focus on ICP pain points, provide value, use ICP language
```

**Prompt Templates**:

**LinkedIn Post Template**:
```
Create a LinkedIn post for [ICP] about [Topic].

Context:
- ICP: [ICP description]
- Messaging: [Key messaging]
- Brand Voice: [Voice and tone]

Requirements:
- Length: [Word count]
- CTA: [CTA]
- Hashtags: [Relevant hashtags]
```

**Blog Post Template**:
```
Create a blog post for [ICP] about [Topic].

Context:
- ICP: [ICP description]
- Messaging: [Key messaging]
- Brand Voice: [Voice and tone]

Requirements:
- Length: [Word count]
- Structure: [Introduction, Body, Conclusion]
- CTA: [Soft CTA]
```

**Email Template**:
```
Create an email for [ICP] about [Topic].

Context:
- ICP: [ICP description]
- Messaging: [Key messaging]
- Brand Voice: [Voice and tone]

Requirements:
- Subject: [Subject line]
- Length: [Word count]
- CTA: [CTA]
```

**Automated Content Generation**:

**Workflow**:
1. Identify content needs (blog posts, social posts, emails)
2. Use base context + prompt templates
3. Generate content with AI
4. Human review and edit
5. Publish and track

**Content Types**:
- Blog posts
- Social media posts
- Email sequences
- Landing page copy
- Ad copy

**Human Review Process**:
- **Review**: Check accuracy, tone, alignment
- **Edit**: Refine messaging, add personality
- **Approve**: Final approval before publishing
- **Track**: Monitor performance

**Content Integration**:
- Channel integration (use content in channels)
- Analytics integration (track content performance)
- Swift CNS integration (feed content data to experiments)

**Document in Swift CNS**:
- Create content development documentation
- Document base context
- Document prompt templates
- Create content experiment plans

### 5. Integrate All Tools with Swift CNS

**Tool Integration Framework**:

**Data Flow**:
1. Tools collect data (analytics, social, content)
2. Data feeds into Swift CNS experiments
3. Experiments track performance
4. Insights synthesized in Swift CNS

**Integration Points**:

**Website → Analytics → Swift CNS**:
- Website events tracked in analytics
- Analytics data feeds Swift CNS experiments
- Website experiments tracked in Swift CNS

**Social → Monitoring → Swift CNS**:
- Social performance tracked in monitoring
- Social data feeds Swift CNS experiments
- Social experiments tracked in Swift CNS

**Content → Analytics → Swift CNS**:
- Content performance tracked in analytics
- Content data feeds Swift CNS experiments
- Content experiments tracked in Swift CNS

**Swift CNS Integration Setup**:
1. Create experiments in Swift CNS
2. Set up data connections (manual or API if available)
3. Track experiment performance
4. Synthesize insights

**Document in Swift CNS**:
- Create tool integration documentation
- Document data flows
- Create experiment tracking plans

## Apply It Now

**Task**: Set up your tool stack

1. Set up website stack (Webflow/Framer/Custom)
2. Set up analytics stack (Mixpanel/Amplitude/PostHog)
3. Set up social monitoring stack (Buffer/Hootsuite)
4. Set up content development stack (ChatGPT/Claude + process)
5. Develop base context for AI prompting
6. Create prompt templates
7. Integrate all tools with Swift CNS

**Artifact**: A complete tool stack setup with:
- Website stack configured
- Analytics stack configured
- Social monitoring stack configured
- Content development stack configured
- All tools integrated with Swift CNS

## Artifacts

You'll create:
- Website stack setup
- Analytics stack setup
- Social monitoring stack setup
- Content development stack setup
- Base context document
- Prompt templates
- Tool integration documentation

## Worked Example

**Situation**: Setting up tool stack for retrospective tool

**Website Stack**:
- Platform: Webflow
- Setup: Account created, website built, domain configured
- Integration: Analytics, forms, UTM tracking

**Analytics Stack**:
- Tool: Mixpanel
- Setup: Account created, SDK installed, events tracked
- Events: Signup, login, feature usage, journey completion
- Dashboards: User activity, feature usage, channel attribution

**Social Monitoring Stack**:
- Tool: Buffer
- Setup: LinkedIn and Twitter connected, posting schedule set
- Monitoring: Mentions, keywords, competitor activity
- Analytics: Track social performance

**Content Development Stack**:
- AI Tool: ChatGPT (GPT-4)
- Base Context:
  - ICP: Engineering Managers at SaaS companies (50-500 employees)
  - Messaging: "Turn retrospectives into action in 30 minutes"
  - Benefits: 50% faster, actionable insights, clear action items
  - Voice: Professional, helpful, direct
- Prompt Templates: LinkedIn posts, blog posts, emails
- Process: Generate → Review → Edit → Publish → Track

**Tool Integration**:
- Website → Analytics → Swift CNS: Track website experiments
- Social → Monitoring → Swift CNS: Track social experiments
- Content → Analytics → Swift CNS: Track content experiments

**Result**: Complete tool stack ready for launch

## Checklist

Before proceeding to the next chapter, verify:
- [ ] Website stack set up (Webflow/Framer/Custom)
- [ ] Analytics stack set up (Mixpanel/Amplitude/PostHog)
- [ ] Social monitoring stack set up (Buffer/Hootsuite)
- [ ] Content development stack set up (AI tools + process)
- [ ] Base context developed
- [ ] Prompt templates created
- [ ] All tools integrated with Swift CNS

## Self-Assessment

1. **What should analytics track?** (Select all)
   - [ ] User signup ✓
   - [ ] Core feature usage ✓
   - [ ] Channel attribution ✓
   - [ ] Every click

2. **What should base context include?**
   - [ ] Only product features
   - [ ] ICP framework + messaging + brand voice ✓
   - [ ] Only messaging
   - [ ] Everything

3. **How should tools integrate?**
   - [ ] Separately
   - [ ] All feed data into Swift CNS experiments ✓
   - [ ] Only analytics
   - [ ] Manually

## Exit Criteria

You're ready to proceed when:
- [ ] Tool stack is complete
- [ ] Analytics tracking is set up
- [ ] Social monitoring is set up
- [ ] Content development process is set up
- [ ] All tools integrated with Swift CNS
- [ ] Ready to launch private beta

## Dependencies & Next Steps

### Prerequisites Completed
- [04 — Build Website V1](04-build-website-v1.md) - Website built

### Next Steps
- Proceed to [06 — Launch Private Beta](06-launch-private-beta.md) to launch private beta
- Use tool stack to track launch performance
- Monitor channels and content through tool stack

### What This Enables

Setting up tool stack enables:
- Performance tracking
- Channel monitoring
- Content creation at scale
- Data-driven decisions
- Experiment tracking
- Insight synthesis

---

> 💡 **Tip**: Start with free tiers. Upgrade as you scale. Focus on tools that integrate with Swift CNS.
> 📝 **Note**: All tools should feed data into Swift CNS experiments. Track everything, synthesize insights.





