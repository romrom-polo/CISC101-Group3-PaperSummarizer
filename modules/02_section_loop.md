# Module 2: Section Loop

## Change Log (2025-11-29)
- Added:
- `summary_level` variable.
- Added conditional logic followed by `summary_level`.

## Responsibilities
- Iterate through each section in order.  
- Summarize each section in <150 words.  
- Ensure summaries are concise, factual, and neutral.  
- Detect problems such as short length or unclear content.  

## Execution Steps
1. For each section:
   - Extract text.
   - If `summary_level` = "short":
        Produce 1-2 sentence compact summary.
   - If `summary_level` = "detailed":
       Produce summary of short paragraph.
       Produce bullet point list of 3-5 key points.
   - Summarize within 150 words.  
   - Check compliance with PS2 constraints.  
2. Store summaries in structured format for rendering.  

