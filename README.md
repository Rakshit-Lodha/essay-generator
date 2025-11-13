AI Content Generator

A multi-stage AI system that generates high-quality content with full control over tone, type, and length. Built with GPT-4o and advanced prompt engineering techniques.

## Features

- **Topic Validation**: Validates input topics before generation to ensure quality
- **Multiple Tones**: Professional, Casual, Technical
- **Multiple Formats**: Blog posts, Social media posts, Emails
- **Length Control**: Short (1 para), Medium (2 paras), Long (3 paras)
- **Quality Assurance**: User satisfaction loop with regeneration option
- **Auto File Saving**: Saves content to UTF-8 encoded text files

## Architecture

The system uses a multi-stage agent architecture:

1. **Validation Agent**: Uses few-shot classification to validate topic quality using GPT 3.5 Turbo
2. **Input Collector**: Structured prompts for tone, type, and length selection
3. **Content Generator**: Chain-of-Thought (CoT) prompting with GPT-4o for quality output
4. **File Saver**: Saves content with proper naming and encoding once you're satisfied with the output

## Performance

**Prompt Engineering Comparison for the main essay generator:**
- **Zero-Shot**: Good output, less consistent with specifications
- **CoT (Selected)**: Better instruction adherence, higher quality output

**Model Selection:**
- **GPT-3.5-turbo**: Tested but inconsistent instruction following
- **GPT-4o (Selected)**: Better quality and specification adherence
