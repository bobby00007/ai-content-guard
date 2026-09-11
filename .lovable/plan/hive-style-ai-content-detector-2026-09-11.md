# Hive-Style AI Content Detector

## Goal
Build a polished, original implementation inspired by Hive’s AI-generated content detection page. The first screen will be the usable detector, not a marketing-only page.

## Experience
- Create a crisp black, white, and electric-lime visual system with bold typography, compact navigation, technical grid details, and restrained motion.
- Keep a Hive-like product structure and tone while using original graphics, wording, and brand marks.
- Make the first viewport an interactive detector with Text and Image tabs, sample inputs, drag-and-drop upload, clear processing states, and responsive layouts.
- Add supporting sections for capabilities, confidence scoring, use cases, trust guidance, and a focused final call to action.

## Detection Features
- **Text:** analyze pasted content and return an overall AI-likelihood score, confidence band, sentence-level highlights, key signals, and a concise interpretation.
- **Images:** analyze uploaded JPG, PNG, or WebP files and return an AI-likelihood score, confidence band, visual-artifact observations, likely generation cues, and an evidence summary.
- Keep access instant with no account requirement or saved history.
- Include input validation, progress states, retry controls, useful empty states, and clear error messages.
- Explain that results are probabilistic signals, not definitive proof.

## Advanced Additions
- Interactive confidence gauge and human-versus-AI distribution.
- Explainability panel with highlighted evidence and weighted signal bars.
- Sample text and sample-image paths so visitors can test immediately.
- Copyable result summary and a printable report view.
- Privacy-first messaging: inputs are processed for the current analysis and not presented as stored history.

## Technical Details
- Use TanStack Start, React, Tailwind design tokens, existing interface primitives, and Lucide icons.
- Add a server-only Lovable AI analysis path using `openai/gpt-6-astra`, with structured results and multimodal image input.
- Validate text length, image MIME type, file size, model output, and all error states before rendering results.
- Stream model work where appropriate, keep the secret server-side, and surface AI service errors directly.
- Add route-specific title, description, Open Graph, and Twitter metadata.
- Verify the real text and image analysis paths, then inspect desktop and mobile rendering for clipping, overlap, and interaction issues.
