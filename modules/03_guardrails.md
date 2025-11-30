# Module 3: Guardrails

## Responsibilities
- Handle missing or empty sections gracefully.  
- Flag sections with <50 words.  
- Prevent hallucination by strictly using provided text.  
- Manage long papers by chunking text into manageable segments.  

## Execution Steps
1. If section missing → mark in "Checks & Warnings".  
2. If section <50 words → flag as short.  
3. Summarize only from provided text; no external sources.  
4. For long papers:
   - Break into chunks.  
   - Maintain context window.  
   - Summarize chunk-by-chunk, then merge.  
