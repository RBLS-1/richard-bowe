# richard-bowe.com Site Reorganization Specification

**Date:** 2026-02-24  
**Purpose:** Restructure portfolio site to better target multiple client types without dilution  
**Strategy:** One domain, targeted landing pages for each service vertical

---

## Executive Summary

**Current problem:** Single site tries to serve trading educators, crypto platforms, iGaming operators, and AI workflow clients with one confused message. Positioning as "Content Systems Architect" alienates trading educators who just need accurate editing.

**Solution:** Keep one domain (richard-bowe.com) but create vertical-specific landing pages that speak directly to each audience type. Main home page becomes broad overview with clear pathways to specialized pages.

**Priority:** Fix critical errors immediately, then build out landing pages over 2-4 weeks.

---

## Critical Fixes Required (Immediate)

### 1. Fix Typos

**Location:** `/about.html`  
**Current:** "My work emsures technical accuracy"  
**Fix:** "My work ensures technical accuracy"

### 2. Verify and Fix Rayner Positioning Claims

**Issue:** Site claims both "Lead Editor" and "ghostwriting" for Rayner Teo.  
**Reality check needed:** Is ghostwriting accurate? If Rich only edits (doesn't write original content), remove all ghostwriting claims.

**Locations to check/fix:**
- `/index.html` - "Lead Editor: Trading with Rayner Teo (2023–Present)"
- `/services.html` - Under "Trading Education Content" mentions ghostwriting
- `/work.html` - "Edit and ghostwrite across options trading..."

**Action:** If NOT ghostwriting, change all instances to "edit" only. If IS ghostwriting, ensure claims are accurate.

### 3. Verify "Top-15 Global Trading Blog" Claim

**Locations:** Multiple pages reference "top-15 trading education blog"  
**Action required:** Verify this ranking is real and citeable. If not verifiable, change to:
- "One of the leading trading education blogs globally" OR
- "Trading education platform with 210,000+ followers" OR
- Remove ranking claim entirely

---

## Site Structure Reorganization

### Current Structure (5 pages - too many)
```
index.html (Home)
about.html (About)
services.html (Services)
work.html (Work)
contact.html (Contact)
```

### New Structure (Hub + Spokes)

```
index.html (Home - hub page, broad positioning)
├── trading-education.html (NEW - Trading educators landing page)
├── crypto-content.html (NEW - Crypto platforms landing page)
├── ai-workflows.html (NEW - AI implementation landing page)
├── igaming-compliance.html (NEW - iGaming operators landing page)
├── work.html (Portfolio - enhanced with filters/sections)
└── contact.html (Contact - simplified)

REMOVE: about.html (fold into home page)
REMOVE: services.html (fold into home page + landing pages)
```

**Why this structure:**
- Home becomes clear "hub" that routes different clients to relevant pages
- Each landing page speaks ONE audience's language
- About/Services content integrated into relevant contexts
- Reduced clicks to conversion
- Better SEO (each landing page targets specific keywords)

---

## Page-by-Page Specifications

### HOME PAGE (index.html) - Rewrite Required

**New Purpose:** Clear hub that identifies your specialization and routes visitors to relevant landing pages

**New Structure:**

#### Header Section
```
<h1>Richard Bowe</h1>
<p class="tagline">Technical Content Specialist for Finance, Crypto & Compliance-Heavy Sectors</p>
```

**Tagline rationale:** Removes confusing "Content Systems Architect" jargon while still showing breadth

#### Opening Paragraph (above the fold)
```
I'm a professional content editor with 3+ years as lead editor for Trading with Rayner Teo, one of the world's leading trading education platforms. My background in Computer Science and 13 years teaching experience means I can verify technical accuracy in complex domains—not just polish grammar.

I specialize in sectors where getting the details wrong has real consequences: trading education, cryptocurrency, DeFi, and high-compliance content like iGaming.
```

#### Core Positioning Section
```html
<section>
    <h2>What I Do</h2>
    <p>I work with three types of clients:</p>
    
    <div class="client-type">
        <h3>Trading & Finance Educators</h3>
        <p>Strategy guides, technical analysis, options trading—edited for mathematical accuracy and pedagogical clarity. I verify the concepts, not just the prose.</p>
        <a href="trading-education.html" class="cta-button">See Trading Work →</a>
    </div>
    
    <div class="client-type">
        <h3>Crypto & DeFi Platforms</h3>
        <p>Blockchain mechanics, protocol documentation, market analysis—30+ months of continuous crypto editing experience with technical accuracy at speed.</p>
        <a href="crypto-content.html" class="cta-button">See Crypto Work →</a>
    </div>
    
    <div class="client-type">
        <h3>High-Compliance Sectors</h3>
        <p>iGaming, automotive, regulated finance—content where regulatory accuracy isn't negotiable. I also build AI content systems for high-volume operations.</p>
        <a href="ai-workflows.html" class="cta-button">See Systems Work →</a>
    </div>
</section>
```

#### Credentials Section
```html
<section>
    <h2>Background</h2>
    <ul>
        <li><strong>Lead Editor:</strong> Trading with Rayner Teo (2023–Present, 500+ articles)</li>
        <li><strong>Crypto Editor:</strong> DSS Digital (2022–Present, 30+ months ongoing)</li>
        <li><strong>AI Architect:</strong> Traffic Lab (2022–Present, 36+ months ongoing)</li>
        <li><strong>Member:</strong> Chartered Institute of Editing and Proofreading (CIEP)</li>
        <li><strong>Education:</strong> Computer Science degree + 13 years teaching experience</li>
        <li><strong>Location:</strong> Japan (JST timezone)</li>
    </ul>
</section>
```

#### Client Retention Proof
```html
<section>
    <h2>Long-Term Reliability</h2>
    <p>My average client relationship is 24+ months. Current ongoing engagements:</p>
    <ul>
        <li>Trading with Rayner: 30+ months</li>
        <li>DSS Digital: 30+ months</li>
        <li>Traffic Lab: 36+ months</li>
        <li>cV Group: 21+ months</li>
    </ul>
</section>
```

#### Simple CTA
```html
<section class="contact-cta">
    <h2>Ready to Work Together?</h2>
    <p>Email: <a href="mailto:rich@richard-bowe.com">rich@richard-bowe.com</a></p>
    <p>Or explore what I can do for your sector:</p>
    <ul>
        <li><a href="trading-education.html">Trading Education</a></li>
        <li><a href="crypto-content.html">Crypto Content</a></li>
        <li><a href="ai-workflows.html">AI & Compliance Systems</a></li>
    </ul>
</section>
```

**Remove from home page:**
- "What Makes My Work Different" bullet points (too abstract)
- Detailed service descriptions (move to landing pages)
- Rate information (keep only on contact page)

---

### TRADING EDUCATION LANDING PAGE (NEW: trading-education.html)

**Purpose:** Convert trading educators specifically (Adam Khoo target audience)

**Target audience:** Trading course creators, financial educators, trading blog owners, proprietary trading firms with education arms

**SEO focus:** "trading content editor," "options trading editor," "technical analysis editor"

#### Header
```
<h1>Professional Editor for Trading Education</h1>
<p class="tagline">Technical accuracy meets pedagogical clarity—I verify the maths, not just the grammar</p>
```

#### Opening Section
```html
<section>
    <p>Most content editors can fix grammar and flow. Few can verify whether your position sizing formula is correct, catch errors in your options Greeks explanation, or ensure your backtest methodology is sound.</p>
    
    <p>I've been the lead editor for Trading with Rayner Teo since 2023—one of the world's leading trading education platforms with 210,000+ followers. Over 500 articles covering options trading, technical analysis, chart patterns, trading psychology, and risk management.</p>
    
    <p>My Computer Science background and domain expertise mean I understand the underlying concepts, not just the surface language. When you explain delta hedging or discuss mean reversion strategies, I can verify accuracy—not just readability.</p>
</section>
```

#### What I Edit Section
```html
<section>
    <h2>What I Edit</h2>
    <ul>
        <li><strong>Trading strategies</strong> - Trend following, mean reversion, breakout systems, momentum</li>
        <li><strong>Technical analysis</strong> - Chart patterns, indicators, price action, support/resistance</li>
        <li><strong>Options trading</strong> - Calls, puts, spreads, Greeks, volatility strategies</li>
        <li><strong>Risk management</strong> - Position sizing, expectancy, drawdown management</li>
        <li><strong>Trading psychology</strong> - Discipline, fear/greed, behavioral patterns</li>
        <li><strong>Market analysis</strong> - Forex, stocks, futures, crypto markets</li>
        <li><strong>Course content</strong> - Video scripts, workbooks, strategy guides, quizzes</li>
    </ul>
</section>
```

#### How I Work Section
```html
<section>
    <h2>How I Work</h2>
    <ul>
        <li><strong>Verify technical accuracy</strong> - Check formulas, validate backtest claims, ensure methodology is sound</li>
        <li><strong>Improve pedagogical structure</strong> - Make complex concepts accessible without dumbing them down</li>
        <li><strong>Maintain your voice</strong> - Edit for clarity while preserving your teaching style</li>
        <li><strong>Scale with you</strong> - From weekly blog posts to full course launches</li>
        <li><strong>Fast turnarounds</strong> - Typical: 24-48 hours for articles, 5-7 days for course modules</li>
    </ul>
</section>
```

#### Case Study: Trading with Rayner Teo
```html
<section>
    <h2>Case Study: Trading with Rayner Teo</h2>
    <p><strong>Challenge:</strong> Maintain technical accuracy across high-volume content production (multiple articles per week) while covering complex topics like options trading, technical analysis, and trading psychology.</p>
    
    <p><strong>Solution:</strong> Lead editor role covering all options trading content plus developmental editing across the platform. Verify mathematical frameworks, check backtest claims, ensure pedagogical clarity.</p>
    
    <p><strong>Results:</strong></p>
    <ul>
        <li>30+ months ongoing partnership (2023–Present)</li>
        <li>500+ articles edited covering strategy, psychology, and technical analysis</li>
        <li>Maintained accuracy across complex topics like expectancy equations and backtested systems</li>
        <li>Supported one of the top trading education platforms globally (210K+ audience)</li>
    </ul>
</section>
```

#### Who This Is For
```html
<section>
    <h2>Who This Is For</h2>
    <p>I'm a good fit if you:</p>
    <ul>
        <li>Run a trading education platform with regular content needs</li>
        <li>Sell courses or coaching that requires technically accurate materials</li>
        <li>Need someone who can verify trading concepts, not just fix typos</li>
        <li>Value long-term relationships over one-off projects</li>
        <li>Want to scale content production without sacrificing quality</li>
    </ul>
    
    <p>I'm probably not the right fit if you need ultra-fast same-day turnarounds or if your content is purely motivational/lifestyle focused.</p>
</section>
```

#### Rates
```html
<section>
    <h2>Investment</h2>
    <p><strong>Standard editing rate:</strong> $50/hour for trading education content</p>
    <p><strong>Typical turnaround:</strong> 24-48 hours for articles (1,500-3,000 words), 5-7 days for course modules</p>
    <p><strong>Monthly retainer options available</strong> for ongoing partnerships (most long-term clients work this way)</p>
</section>
```

#### CTA
```html
<section class="contact-cta">
    <h2>Let's Talk</h2>
    <p>If you need an editor who understands trading as well as writing, let's discuss your project.</p>
    <p><strong>Email:</strong> <a href="mailto:rich@richard-bowe.com">rich@richard-bowe.com</a></p>
    <p>In your message, briefly describe your content needs, volume, and cadence. I'll come back within one business day with honest feedback on fit.</p>
</section>
```

**Deliberately exclude from this page:**
- Casino/iGaming work
- Crypto work (unless tangentially relevant like "crypto trading education")
- AI workflow architecture (not relevant to this audience)
- Generic proofreading services

---

### CRYPTO CONTENT LANDING PAGE (NEW: crypto-content.html)

**Purpose:** Convert crypto platforms, DeFi projects, blockchain publications

**Target audience:** Crypto news sites, DeFi protocol teams, blockchain analytics platforms, crypto trading platforms

**SEO focus:** "crypto content editor," "DeFi editor," "blockchain content"

#### Header
```
<h1>Crypto Content Editor with 30+ Months Proven Track Record</h1>
<p class="tagline">Technical accuracy for blockchain mechanics, DeFi protocols, and market analysis—at speed</p>
```

#### Opening
```html
<section>
    <p>Crypto content moves fast. Protocols launch, markets shift, and technical details matter. You need an editor who understands blockchain mechanics well enough to catch errors in protocol explanations, verify tokenomics claims, and maintain accuracy across market cycles.</p>
    
    <p>I've been editing crypto content weekly for DSS Digital since 2022—30+ continuous months covering DeFi protocols, blockchain technology, and cryptocurrency markets. My Computer Science background means I can verify technical claims about consensus mechanisms, smart contracts, and on-chain data—not just polish the grammar.</p>
</section>
```

#### What I Edit
```html
<section>
    <h2>What I Edit</h2>
    <ul>
        <li><strong>Blockchain technology</strong> - Consensus mechanisms, protocol architecture, layer-2 solutions</li>
        <li><strong>DeFi protocols</strong> - Lending, staking, liquidity pools, yield farming, governance</li>
        <li><strong>Market analysis</strong> - Technical analysis for crypto, market trends, trading strategies</li>
        <li><strong>Tokenomics</strong> - Token distribution, utility, incentive mechanisms</li>
        <li><strong>NFTs & Web3</strong> - Digital ownership, smart contracts, gaming applications</li>
        <li><strong>Regulatory content</strong> - Compliance, legal frameworks (with appropriate disclaimers)</li>
    </ul>
</section>
```

#### Case Study: DSS Digital
```html
<section>
    <h2>Case Study: DSS Digital</h2>
    <p><strong>Challenge:</strong> Weekly crypto content editing with fast turnarounds in a rapidly evolving space where technical accuracy can't slip.</p>
    
    <p><strong>Solution:</strong> Ongoing editing engagement covering blockchain mechanics, DeFi protocols, and cryptocurrency markets. Verify technical claims, check protocol details, maintain clarity for mixed-expertise audiences.</p>
    
    <p><strong>Results:</strong></p>
    <ul>
        <li>30+ months continuous engagement (2022–Present)</li>
        <li>Consistent weekly delivery across market ups and downs</li>
        <li>Technical accuracy maintained across protocol launches, market events, and regulatory changes</li>
        <li>Long-term reliability in a sector known for high editor turnover</li>
    </ul>
</section>
```

#### Additional Crypto Experience
```html
<section>
    <h2>Additional Crypto Experience</h2>
    
    <div class="project">
        <h3>POW3R MEDIA Network (NFT Plazas, NFT Insider, MagNFT)</h3>
        <p><strong>Role:</strong> Web3 Journalist & Editor (2024-2025)</p>
        <p>GameFi reviews, NFT collection analysis, blockchain gaming coverage. BBC-style neutral reporting across play-to-earn mechanics, digital ownership, and community sentiment.</p>
    </div>
    
    <div class="project">
        <h3>HFDX DeFi Exchange (Allcaps Agency)</h3>
        <p><strong>Role:</strong> Project Manager + Senior Writer</p>
        <p>47 articles for decentralized perpetual exchange. Managed team of 4 writers. Covered infrastructure reliability, institutional positioning, and DeFi derivatives trading.</p>
    </div>
</section>
```

#### Rates & CTA
```html
<section>
    <h2>Investment</h2>
    <p><strong>Crypto editing rate:</strong> $50-60/hour depending on technical complexity</p>
    <p><strong>Typical turnaround:</strong> 24-48 hours for articles, 3-5 days for protocol documentation</p>
</section>

<section class="contact-cta">
    <h2>Let's Talk</h2>
    <p>Need a crypto editor who can keep up with your pace and verify your technical claims?</p>
    <p><strong>Email:</strong> <a href="mailto:rich@richard-bowe.com">rich@richard-bowe.com</a></p>
</section>
```

---

### AI WORKFLOWS & COMPLIANCE LANDING PAGE (NEW: ai-workflows.html)

**Purpose:** Convert companies implementing AI content systems and high-compliance operators

**Target audience:** iGaming operators, content agencies scaling with AI, regulated platforms, automotive content platforms

**SEO focus:** "AI content systems," "LLM workflow design," "compliance content editor"

#### Header
```
<h1>AI Content Systems & High-Compliance Editorial</h1>
<p class="tagline">Building scalable content pipelines for iGaming, compliance-heavy sectors, and AI-augmented operations</p>
```

#### Opening
```html
<section>
    <p>If you're implementing AI content systems or operating in sectors where compliance errors have real consequences, you need someone who understands both the technical architecture and the editorial standards.</p>
    
    <p>I've spent 36+ months designing and maintaining AI-augmented content systems for Traffic Lab (iGaming sector), built LLM pipelines for Berlitz's language education platform, and edited high-compliance content across automotive and finance sectors.</p>
    
    <p>I build the systems that produce consistent, compliant content at scale—not just write individual pieces.</p>
</section>
```

#### Services Section
```html
<section>
    <h2>What I Build</h2>
    
    <div class="service">
        <h3>AI Content Pipeline Design</h3>
        <ul>
            <li>Custom LLM workflows (GPT, Claude, Gemini)</li>
            <li>Multi-stage quality control frameworks</li>
            <li>Anti-plagiarism and fact-checking protocols</li>
            <li>Human-in-the-loop editorial layers</li>
            <li>Python automation for content operations</li>
        </ul>
    </div>
    
    <div class="service">
        <h3>High-Compliance Content Editing</h3>
        <ul>
            <li><strong>iGaming:</strong> Casino reviews, licensing verification, bonus term accuracy</li>
            <li><strong>Automotive:</strong> Technical specifications, regulatory compliance</li>
            <li><strong>DeFi:</strong> Protocol accuracy, risk disclosures</li>
            <li><strong>Finance:</strong> Regulatory claims, compliance terminology</li>
        </ul>
    </div>
</section>
```

#### Case Study: Traffic Lab
```html
<section>
    <h2>Case Study: Traffic Lab (iGaming AI Systems)</h2>
    <p><strong>Challenge:</strong> Scale casino review production while maintaining regulatory compliance and editorial quality in a legally sensitive vertical.</p>
    
    <p><strong>Solution:</strong> Designed AI-augmented content system evolving from custom GPT to two-stage Gemini Deep Research pipeline. Built quality control frameworks, compliance checks, and editorial review layers.</p>
    
    <p><strong>Results:</strong></p>
    <ul>
        <li>36+ months ongoing engagement (2022–Present)</li>
        <li>Reduced per-review production time while maintaining compliance standards</li>
        <li>Systems adapted across multiple LLM generations (GPT-3.5 → GPT-4 → Gemini)</li>
        <li>Zero compliance issues from AI-generated content</li>
    </ul>
</section>
```

#### Case Study: Berlitz
```html
<section>
    <h2>Case Study: Berlitz (AI Prompt Engineering)</h2>
    <p><strong>Challenge:</strong> Design prompts for language tutor LLM that produce pedagogically sound instruction at scale.</p>
    
    <p><strong>Solution:</strong> Applied 13+ years teaching experience to prompt engineering—balancing naturalness, accuracy, and learner-appropriate tone for one of the world's largest language education organisations.</p>
    
    <p><strong>Outcome:</strong> Effective prompts combining technical AI expertise with deep pedagogical knowledge.</p>
</section>
```

#### Who This Is For
```html
<section>
    <h2>Who This Is For</h2>
    <p>I'm a good fit if you:</p>
    <ul>
        <li>Need to implement AI content systems but want quality control built in</li>
        <li>Operate in compliance-heavy sectors (iGaming, finance, automotive, pharma)</li>
        <li>Want to scale content production without sacrificing regulatory accuracy</li>
        <li>Need both the technical implementation AND the editorial standards</li>
        <li>Value long-term system maintenance over one-off builds</li>
    </ul>
</section>
```

#### Rates & CTA
```html
<section>
    <h2>Investment</h2>
    <p><strong>AI workflow design:</strong> $60-80/hour</p>
    <p><strong>Compliance editing:</strong> $50-70/hour</p>
    <p><strong>Project-based pricing available</strong> for system builds</p>
</section>

<section class="contact-cta">
    <h2>Ready to Build?</h2>
    <p>Tell me about your content challenges and I'll let you know if we're a good fit.</p>
    <p><strong>Email:</strong> <a href="mailto:rich@richard-bowe.com">rich@richard-bowe.com</a></p>
</section>
```

---

### WORK PAGE (work.html) - Enhanced Version

**Purpose:** Comprehensive portfolio showing all work with filters/sections

**Keep current structure but enhance with:**

#### Section Navigation
```html
<nav class="work-filter">
    <a href="#trading">Trading Education</a>
    <a href="#crypto">Crypto & DeFi</a>
    <a href="#ai-systems">AI & Compliance Systems</a>
    <a href="#all">All Projects</a>
</nav>
```

#### Organize projects into clear sections
```html
<section id="trading">
    <h2>Trading Education</h2>
    <!-- Trading with Rayner project -->
</section>

<section id="crypto">
    <h2>Crypto & DeFi</h2>
    <!-- DSS Digital, POW3R MEDIA, HFDX projects -->
</section>

<section id="ai-systems">
    <h2>AI Systems & Compliance</h2>
    <!-- Traffic Lab, Berlitz, CarVertical projects -->
</section>
```

**Keep all existing project content** but organize it better.

---

### CONTACT PAGE (contact.html) - Simplified

**Purpose:** Easy, clear way to get in touch

**Simplify to:**

```html
<section>
    <h2>Get in Touch</h2>
    <p>The best way to reach me is by email. I respond within one business day.</p>
    <p><strong>Email:</strong> <a href="mailto:rich@richard-bowe.com">rich@richard-bowe.com</a></p>
    
    <p>In your message, it helps to include:</p>
    <ul>
        <li>Brief description of your project or content needs</li>
        <li>Volume and cadence you're working to</li>
        <li>What sector/niche (trading, crypto, iGaming, etc.)</li>
    </ul>
    
    <p>I'll come back with honest feedback on fit and, if appropriate, a proposal.</p>
</section>

<section>
    <h2>Rates</h2>
    <table class="rate-table">
        <thead>
            <tr>
                <th>Service</th>
                <th>Rate</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Proofreading & copy editing</td>
                <td>$30–40/hr</td>
            </tr>
            <tr>
                <td>Trading education content editing</td>
                <td>$50/hr</td>
            </tr>
            <tr>
                <td>Crypto/DeFi content editing</td>
                <td>$50–60/hr</td>
            </tr>
            <tr>
                <td>High-compliance editing (iGaming, automotive)</td>
                <td>$50–70/hr</td>
            </tr>
            <tr>
                <td>AI workflow design & systems architecture</td>
                <td>$60–80/hr</td>
            </tr>
        </tbody>
    </table>
    <p>Monthly retainer pricing available for ongoing engagements. Most long-term clients work this way after an initial project.</p>
</section>

<section>
    <h2>Location & Availability</h2>
    <ul>
        <li><strong>Based:</strong> Japan</li>
        <li><strong>Timezone:</strong> JST (UTC+9)</li>
        <li><strong>Response time:</strong> Within one business day</li>
    </ul>
</section>
```

**Remove:** "Who I Work Best With" section (too defensive, move to landing pages if needed)

---

## Content Writing Guidelines

### Tone & Style Rules

**DO:**
- Use British English throughout
- Write in first person ("I edit..." not "Rich edits...")
- Be direct and specific
- Lead with proof (client names, durations, metrics)
- Use concrete examples over abstract benefits
- Keep sentences clear and scannable

**DON'T:**
- Use corporate jargon ("synergies," "leverage," "ideate")
- Make unverifiable claims
- Hide behind passive voice
- Use excessive modifiers ("very," "really," "quite")
- Create artificial sections just to fill space

### Word Choices to Avoid
- "Synergies"
- "Leverage" (as verb)
- "Ideate"
- "Deliverables" (unless necessary)
- "Solutions" (overused)
- "World-class" (prove it instead)
- "Cutting-edge" (meaningless)

### Proof Over Claims
**Bad:** "I provide world-class editing services"  
**Good:** "30+ months continuous engagement with DSS Digital"

**Bad:** "I'm an expert in trading content"  
**Good:** "Lead editor for Trading with Rayner Teo—500+ articles covering options, technical analysis, and trading psychology"

---

## Technical Implementation Notes

### SEO Considerations

**Each landing page should target:**
- Primary keyword in H1
- Secondary keywords in H2s
- Long-tail variations in body content
- Internal links to relevant work examples
- Clear meta descriptions

**Example meta descriptions:**

```html
<!-- trading-education.html -->
<meta name="description" content="Professional trading content editor with 3+ years editing for Rayner Teo. Technical accuracy for options, technical analysis, and strategy guides. $50/hr.">

<!-- crypto-content.html -->
<meta name="description" content="Crypto content editor with 30+ months proven track record. DeFi protocols, blockchain mechanics, market analysis. Fast turnarounds with technical accuracy.">

<!-- ai-workflows.html -->
<meta name="description" content="AI content system architect for iGaming and compliance-heavy sectors. 36+ months designing LLM pipelines with quality control frameworks.">
```

### Navigation Updates

Update main navigation to include landing pages:

```html
<nav>
    <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="trading-education.html">Trading</a></li>
        <li><a href="crypto-content.html">Crypto</a></li>
        <li><a href="ai-workflows.html">AI & Compliance</a></li>
        <li><a href="work.html">Work</a></li>
        <li><a href="contact.html">Contact</a></li>
    </ul>
</nav>
```

### Internal Linking Strategy

**From home page:**
- Link "trading educators" → trading-education.html
- Link "crypto platforms" → crypto-content.html
- Link "AI systems" → ai-workflows.html
- Link specific project mentions → work.html#projectname

**From landing pages:**
- Link back to home for breadth
- Link to work.html for portfolio depth
- Link to contact.html for conversion
- Cross-link between landing pages where relevant (e.g., "crypto trading education" could link trading ↔ crypto pages)

### URL Structure (Clean URLs)

If possible, configure server for clean URLs:
```
/trading-education (instead of /trading-education.html)
/crypto-content (instead of /crypto-content.html)
/ai-workflows (instead of /ai-workflows.html)
```

If not possible, .html extensions are fine.

---

## Files to Delete

**Remove these files:**
- `about.html` (content folded into index.html and landing pages)
- `services.html` (content folded into landing pages)

---

## Implementation Checklist

### Phase 1: Critical Fixes (Do First)
- [ ] Fix "emsures" typo on about.html
- [ ] Verify and correct Rayner "ghostwriting" claims
- [ ] Verify "top-15 blog" ranking claim
- [ ] Remove unverifiable claims

### Phase 2: Home Page Rebuild
- [ ] Rewrite index.html per spec above
- [ ] Update tagline
- [ ] Create clear routing to landing pages
- [ ] Add credentials section
- [ ] Add client retention proof
- [ ] Simplify CTA

### Phase 3: Landing Pages (Priority Order)
1. [ ] Create trading-education.html (HIGHEST PRIORITY—needed for Adam Khoo)
2. [ ] Create crypto-content.html
3. [ ] Create ai-workflows.html

### Phase 4: Supporting Pages
- [ ] Enhance work.html with section filters
- [ ] Simplify contact.html
- [ ] Delete about.html
- [ ] Delete services.html

### Phase 5: Technical
- [ ] Update navigation on all pages
- [ ] Update meta descriptions
- [ ] Implement internal linking
- [ ] Test all links
- [ ] Verify mobile responsiveness
- [ ] Check page load speeds

### Phase 6: Polish
- [ ] Proofread all new content
- [ ] Verify British English throughout
- [ ] Check for consistency in claims across pages
- [ ] Test conversion paths (home → landing → contact)
- [ ] Get feedback from trusted source

---

## Success Metrics

**How to know this worked:**

1. **Bounce rate by landing page** - Are people staying on vertical-specific pages longer than old generic pages?
2. **Conversion tracking** - Are you getting more enquiries from specific verticals?
3. **Email quality** - Are enquiries more qualified (people already know what you do)?
4. **Client feedback** - When prospects email, do they reference the specific landing page?

**Target outcome:**
- Trading educators land on /trading-education and immediately see Rayner credential
- Crypto platforms land on /crypto-content and see 30+ months proof
- AI implementers land on /ai-workflows and see systems expertise
- All paths feel natural and specialized, not generic

---

## Final Notes

**This is a "hub and spokes" architecture:**
- Home = hub (shows breadth, routes to specializations)
- Landing pages = spokes (show depth, convert specific audiences)
- Work = portfolio (proves claims across all spokes)
- Contact = conversion point (simple, clear, rates transparent)

**The goal is NOT to hide your range**—it's to lead with the most relevant expertise for each visitor.

Someone looking for a trading editor sees trading expertise first. If they want to verify you can handle complexity, they can explore crypto/AI work as supporting proof. But they're not confused by it on first contact.

**Priority:** Build trading-education.html FIRST. That's needed for Adam Khoo and will serve as template for other landing pages.