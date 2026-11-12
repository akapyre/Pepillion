# Pepillion

A daily peptide trivia game where you dive into a volcano. Each day gives 7 prompts ("Name a GLP-1–based drug", "Name a peptide studied for longevity"…), picked from 20 categories. Every correct answer sinks you deeper, from the Crater Rim down to the Core Forge, and rarer answers sink you further (common +150 m up to deep cut +900 m). Some answers look right but aren't peptides (MK-677, creatine, testosterone). Those score nothing and explain why.

- `index.html` is the whole game. Open it in a browser.
- The prompt bank lives in the `PROMPTS` array at the top of the script. Each answer is `[tier, "Display name", ...aliases]`, with tier 1 (common) to 4 (deep cut). Each trap is `["Name", "Why it doesn't count", ...aliases]`.
- When hosted as a Claude artifact with the `db` capability, rarity comes from what other players answered that day, once at least 8 have played. Otherwise it uses the built-in tiers.

For education only. Not medical advice.
