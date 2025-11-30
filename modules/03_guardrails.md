# Module 3: Guardrails

## Change Log (2025-11-29)
- Added strict evidence logic.
- Added standardized warning messages for missing/short sections & strict mod.

## Responsibilities
- Handle missing or empty sections gracefully.  
- Flag sections with <50 words.  
- Prevent hallucination by strictly using provided text.  
- Manage long papers by chunking text into manageable segments.  

## Execution Steps
1. If section is missing or empty:
      print “Section skipped: no usable text was provided.”.  
3. If section <50 words:
      print “Section very short: summary may be incomplete.”.
4. If evidence_mode = "strict":
      ONLY use informations, claims, equations provided from the text.
   If text does not include enough information:
      print “The source text does not provide enough detail to summarize this section in strict evidence mode.”
5. For long papers:
   - Break into chunks.  
   - Maintain context window.  
   - Summarize chunk-by-chunk, then merge.  

