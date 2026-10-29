# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

## AIM
To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.

## Scenario:
You are part of a content curation team for an educational platform that delivers quick summaries of research papers to undergraduate students. Your task is to summarize a 500-word technical article on "The Basics of Blockchain Technology" using multiple AI platforms and prompting strategies.

Your goal is to determine which combination of prompting technique + platform provides the best summary in terms of:

- Accuracy
- Coherence
- Simplicity
- Speed
- User experience

## Algorithm

1. Select a 500-word technical article on "The Basics of Blockchain Technology" as the source text.
2. Choose four AI platforms: ChatGPT, Gemini, Claude, and Copilot.
3. Design four prompts for the same summarization task:
   - **Zero-shot:** a direct instruction with no examples.
   - **Few-shot:** the instruction plus two worked examples (AI and Cloud Computing).
   - **Chain-of-Thought:** a six-step reasoning guide (identify the topic, list the concepts, find the benefits, remove jargon, simplify, combine) with a 120-150 word limit.
   - **Role-based:** the model acts as an educational content curator with a defined audience and output format.
4. Run every prompt on every platform (4 techniques x 4 platforms = 16 outputs) and record each response.
5. Score each output from 1 to 5 on Accuracy, Coherence, Simplicity, Speed, and User Experience.
6. Total the scores per output, per technique, and per platform.
7. Compare the totals to identify the best technique, the best platform, and the best combination.

## Output

### Summary of the outputs generated

| Technique | ChatGPT | Gemini | Claude | Copilot |
|---|---|---|---|---|
| Zero-shot | Short 3-paragraph summary covering decentralization, transparency, and uses | Longest answer, with numbered concepts (blocks, hash, nodes, consensus) | Notebook analogy with headed sections | Bullet-style summary that includes challenges (energy use, slow speed) |
| Few-shot | One compact paragraph that follows the example style | Short structured summary with "How It Works" and "Why It Matters" | Very concise single paragraph | Simple "Blockchain Made Simple" layout |
| Chain-of-Thought | Clear 120-150 word paragraph | Concise, with a key-benefits list | Well-organized 3-paragraph summary within the word limit | Summary with benefits and limitations |
| Role-based | Clear, student-friendly paragraphs | Structured guide: How It Works, Why It Matters | Engaging, analogy-based, and complete | Detailed summary with smart contracts and challenges |

### Evaluation scores (1-5)

| Technique | Platform | Accuracy | Coherence | Simplicity | Speed | UX | Total (/25) |
|---|---|---|---|---|---|---|---|
| Zero-shot | ChatGPT | 4 | 4 | 5 | 5 | 4 | 22 |
| Zero-shot | Gemini | 5 | 4 | 3 | 4 | 4 | 20 |
| Zero-shot | Claude | 5 | 5 | 4 | 3 | 5 | 22 |
| Zero-shot | Copilot | 4 | 4 | 4 | 4 | 5 | 21 |
| Few-shot | ChatGPT | 4 | 4 | 5 | 5 | 4 | 22 |
| Few-shot | Gemini | 5 | 5 | 4 | 3 | 5 | 22 |
| Few-shot | Claude | 5 | 5 | 5 | 3 | 5 | 23 |
| Few-shot | Copilot | 4 | 4 | 4 | 4 | 5 | 21 |
| Chain-of-Thought | ChatGPT | 4 | 5 | 4 | 4 | 4 | 21 |
| Chain-of-Thought | Gemini | 5 | 5 | 4 | 3 | 5 | 22 |
| Chain-of-Thought | Claude | 5 | 5 | 5 | 4 | 5 | 24 |
| Chain-of-Thought | Copilot | 4 | 4 | 4 | 4 | 5 | 21 |
| Role-based | ChatGPT | 4 | 5 | 5 | 5 | 5 | 24 |
| Role-based | Gemini | 5 | 5 | 5 | 4 | 5 | 24 |
| Role-based | Claude | 5 | 5 | 5 | 4 | 5 | 24 |
| Role-based | Copilot | 4 | 4 | 5 | 4 | 5 | 22 |

### Totals

| Technique | ChatGPT | Gemini | Claude | Copilot | Technique Total |
|---|---|---|---|---|---|
| Zero-shot | 22 | 20 | 22 | 21 | 85 |
| Few-shot | 22 | 22 | 23 | 21 | 88 |
| Chain-of-Thought | 21 | 22 | 24 | 21 | 88 |
| Role-based | 24 | 24 | 24 | 22 | 94 |
| **Platform Total** | 89 | 88 | **93** | 85 | |

## Result

- **Best AI platform: Claude** (93/100). It scored 5/5 on accuracy and coherence in every technique and was the most consistent across prompts.
- **Best prompting technique:** Role-based had the highest overall total (94), and Chain-of-Thought gave the strongest result on the best platform (Claude 24/25). Zero-shot was the
