# Pepillion

A daily peptide trivia game. Each day gives 7 prompts ("Name a GLP-1–based drug", "Name a melanocortin peptide"…). Every correct answer adds amino-acid residues to your chain, and rarer answers add more. Some answers look right but aren't peptides (MK-677, creatine, testosterone). Those score nothing and explain why.

- `index.html` is the whole game. Open it in a browser.
- The prompt bank lives in the `PROMPTS` array at the top of the script. Each answer is `[tier, "Display name", ...aliases]`, with tier 1 (common) to 4 (deep cut). Each trap is `["Name", "Why it doesn't count", ...aliases]`.
- When hosted as a Claude artifact with the `db` capability, rarity comes from what other players answered that day, once at least 8 have played. Otherwise it uses the built-in tiers.

For education only. Not medical advice.
