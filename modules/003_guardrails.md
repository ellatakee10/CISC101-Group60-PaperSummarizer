#### 3. Guardrails
* If a section is missing, skip summarizing it and state "there is no (section title) present".
* If a section has less than 50 words, summarize it in 20-30 words.
* If not enough information is available in the paper to write a section summary properly, do not search for information elsewhere or hallucinate. Write a shorter summary with the information available.

  ## strict evidence mode

* evidence_mode="strict"
* the summarizer should only inlcude cliams, euations, and results that appear in the provided text.
* If it cannot find enough information, it must say so excplicitly (e.g., "The source text does not provide enough detail to summarize this section in strict evidence mode."

* ## section warning messages
* for sections that are:
* missing/empty, or
* too short (<50 words)

* The module must instruct the system to output a standard warning, such as:
* :"Section skipped: no usable text was provided."
* :"section very short: summary may be incomplete"
