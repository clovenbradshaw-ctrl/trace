# TRACE Badge Generator v1.1.0

**Transparent Reporting of AI Contributions & Edits**

A web-based tool for creating transparency badges that disclose AI assistance in creative and professional work.

## Links
- **Badge Generator Widget**: [Available here](https://clovenbradshaw-ctrl.github.io/trace/)

## Why TRACE Matters

With AI tools becoming ubiquitous in our workflows, transparency has become critical. Recent findings from BipartisanPolicy.org revealed a significant negative correlation between frequent AI tool usage and critical thinking abilities, mediated by increased cognitive offloading. Younger participants exhibited higher dependence on AI tools and lower critical thinking scores compared to older participants.

Yet virtually nothing we work on doesn't touch, in some way, a large language model. From deep research and analysis to proofreading for typos, from coding assistance to creative generation—AI is everywhere. It feels weird to say "yes, I made this" without acknowledging the AI's role, but it's also clunky to just say "yeah, I used some AI."

TRACE provides a structured, visual way to disclose precisely when and how AI tools contributed to any piece of work.

## Philosophy

Socrates worried that writing would ruin memory. He wasn't wrong—oral traditions that once carried epics across generations shrank to quaint performances. People stopped remembering because remembering was no longer required. But that ruin rewired us. Once thoughts could be written, they could be compared, cross-referenced, argued over. We lost memory, but we gained history.

The same pattern is here again. Large language models will ruin something, and they will rewire something. They will corrode habits of critical thinking in the same way books corroded memory. As the article above cites, this could have concerning consequences on our critical thinking skills. But the trade will open new terrain—architectures of knowledge and prosthetics for thought.

The danger isn't just in the ruin, or even in the rewiring. It's in pretending one comes without the other. In mistaking sand for stone. In waking up amid the ruins, unable to remember how we got there.

That's why experiments like TRACE matter. Not because they prevent the ruin, but because they mark it. They admit the handoffs: here the ghost drafted, here the hive mind synthesized, here I proofed and steered. Imperfect, bureaucratic, even clumsy—but at least an honest record of what happened.

## What is TRACE?

TRACE is a framework for transparent AI disclosure that creates visual badges and citations documenting exactly how AI was used in any piece of work. Every AI-touched project gets a four-quadrant badge showing:

### 1. DATA - What sources were given?
The information foundation that shaped the AI's response. This quadrant discloses whether the AI worked with publicly verifiable information, proprietary materials, or relied solely on its training data.

- **Public**: Only openly available information, URLs, or user-created prompts
- **Internal**: Private, proprietary, or paywalled materials  
- **Model-only**: No external inputs provided; relied on pre-trained knowledge
- **Unclear**: Source attribution is uncertain or unknowable

### 2. ROLE - What job did the AI do?
The primary function the AI performed in creating the content. This quadrant reveals the degree of AI involvement, from light editing to full generation.

- **Assist**: Cleaned up grammar, spelling, style, or formatting
- **Draft**: Generated the main body of content
- **Synthesis**: Combined or merged multiple provided sources
- **Analysis**: Explained patterns, performed calculations, or reasoned through problems
- **Exploratory**: Used experimentally without fixed goals
- **Creative**: Invented original content, narratives, or artistic elements

### 3. METHODOLOGY - How was the job carried out?
The workflow and techniques used to produce the output. This quadrant describes the complexity and structure of the AI interaction.

- **Raw Response**: Published the first output with minimal editing
- **Guided**: Structured the task with steps, scaffolding, or context
- **Rewriter**: Transformed existing text into a new format or style
- **Augmented**: Used external tools, plugins, or environments beyond the base model

### 4. REVIEW - How was the output checked?
The level and type of human oversight applied after generation. This quadrant indicates the verification and quality control measures taken.

- **Unreviewed**: No human checked the output before use
- **Skimmed**: Quick review for tone and obvious issues only
- **Peer Review**: Non-expert but knowledgeable person reviewed carefully
- **Expert Review**: Subject-matter expert verified accuracy and quality
- **AI Self-Check**: The model was prompted to critique or improve its own output

Each quadrant works together to create a complete picture of how AI was integrated into the content creation process, promoting transparency and helping both creators and audiences understand the human-AI collaboration involved.

## Features

- **Visual Badge Generation**: Four-quadrant colored badge displaying TRACE codes
- **Natural Language Citations**: Human-readable disclosure statements
- **AI Model Database**: 200+ models via OpenRouter API
- **Export Options**: PNG badges and clipboard-ready citations
- **Customizable Display**: Color/grayscale, label visibility options

## Common Use Cases

### Deep Research
Using tools from Anthropic and OpenAI for analysis and citations on topics that are difficult or impossible to "just Google about."
- Typical badge: `P-Analysis-Guided-Expert`

### Proofreading
Finding typos and homophone replacements (they're/their, its/it's) that verbal learners often miss.
- Typical badge: `Model-Assist-Raw-Skimmed`

### Code Development
Building interactive charts and mini-websites with coding assistant tools.
- Typical badge: `Public-Creative-Augmented-Peer`

### Content Creation
Generating drafts for blog posts, reports, or creative writing.
- Typical badge: `Public-Draft-Guided-Skimmed`

## Quick Start

1. Open the TRACE badge generator in your browser
2. Select options from each quadrant:
   - Choose your data source type
   - Define the AI's role
   - Specify your methodology
   - Indicate review level
3. (Optional) Add specific AI models used
4. Download badge or copy citation

## Installation

### Option 1: Web Widget
Visit the online generator at [widget URL]

### Option 2: Local HTML File
```bash
# Download the HTML file
# Open directly in browser or serve locally:

# Python
python -m http.server 8000

# Node.js
npx http-server
```

## Example Badges & Citations

### Research Paper
**Badge Code**: `PI-Analysis-Guided-Expert`
**Citation**: "AI assisted in analyzing patterns using both public and internal data sources through guided prompting. The output underwent expert review."

### Blog Post  
**Badge Code**: `P-Draft-Rewriter-Skimmed`
**Citation**: "AI drafted content from public sources using a rewriting methodology. The output received a quick review for tone and obvious issues."

### Technical Documentation
**Badge Code**: `M-Synthesis-Augmented-Peer`
**Citation**: "AI synthesized information from its training data using augmented tools. A knowledgeable colleague reviewed the output carefully."

## Technical Details

- **Version**: 1.1.0
- **Dependencies**: html2canvas for PNG export
- **API**: OpenRouter models (via CORS proxy)
- **Compatibility**: Chrome 90+, Firefox 88+, Safari 14+
- **License**: Open source for transparency promotion

## Privacy & Ethics

- All processing happens locally in your browser
- No data stored or transmitted to external servers
- Promotes ethical AI use through radical transparency
- Helps track human-AI collaboration patterns
- Enables accountability in AI-assisted work

## Why Transparency Matters Now

Most of us are already using AI heavily. The newer coding tools are invaluable. Research assistants provide analysis we couldn't achieve alone. Proofreaders catch errors our brains skip over. But without disclosure:

- We risk eroding trust in creative and professional work
- We lose track of our own cognitive dependencies  
- We can't study what we're losing and gaining
- We participate in a kind of collective amnesia about how work gets done

TRACE isn't about shaming AI use or celebrating it. It's about honest accounting—marking where the human ended and the machine began, so we can at least remember how we got here.

## Contributing

This tool is designed to evolve with community input. Key areas for contribution:
- Refining category definitions based on industry needs
- Improving natural language templates
- Adding export formats and integrations
- Developing industry-specific variations
- Creating plugins for common platforms
- Building automation tools for badge generation

## Citation Format

When using TRACE badges in your work:
```
AI Disclosure: TRACE framework [Badge Code]
Transparent Reporting of AI Contributions & Edits
Generated: [date]
Details: [natural language description]
```

## Support & Troubleshooting

- Check browser console for JavaScript errors
- Ensure JavaScript is enabled
- Try local server for CORS issues
- Models list falls back gracefully if API unavailable
- Clear cache if badge generation fails

## Future Roadmap

- Integration with major publishing platforms
- Automated detection suggestions
- Collaborative review workflows  
- Industry-specific templates
- API for programmatic badge generation
- Browser extensions for easy insertion

-------------------------
AI Disclosure (2025-08-28)
TRACE: S-P-G-P

Role: Synthesis
Data: Public
Method: Guided
Review: Peer

AI Models Used:
• Anthropic: Claude Opus 4.1 (anthropic/claude-opus-4.1)

I used AI to synthesize information from multiple sources using public sources, through guided prompting. The output underwent peer review. The AI model used was Anthropic: Claude Opus 4.1.
-------------------------

*Because the danger isn't in using AI—it's in pretending we're not.*

**Version**: 1.1.0  
**Last Updated**: August 2025  
**Framework**: TRACE (Transparent Reporting of AI Contributions & Edits)
**Copyright**: Michael Lacy
