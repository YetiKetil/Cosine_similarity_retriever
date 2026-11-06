# Survey Item Similarity Calculator (Colab)

Compute pairwise semantic similarity between survey/questionnaire items using
OpenAI, Voyage AI or Claude – or a free local model that needs no API key.
Python/Colab port of the SwiftUI app *SurveySimilarity*; runs on any computer with a browser.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YetiKetil/Cosine_similarity_retriever/blob/main/SurveySimilarity.ipynb)

## Methods

| Method | Model | Key |
|---|---|---|
| Local (offline) | `all-MiniLM-L6-v2` (sentence-transformers) | none |
| OpenAI Small / Large | `text-embedding-3-small` / `-large` | `OPENAI_API_KEY` |
| Voyage AI | `voyage-3` | `VOYAGE_API_KEY` |
| Claude (Semantic) | Claude rates each pair 0.0–1.0 | `ANTHROPIC_API_KEY` |

## Quick start

1. Click **Open in Colab** above (or *File → Open notebook → GitHub* in Colab).
2. Add your own API keys under 🔑 **Secrets** in Colab's left sidebar (names as above) and enable notebook access.
3. Paste your items in step 2, choose `METHODS` in step 3, then *Runtime → Run all*.
4. Results appear as list, matrix and heatmap; CSV files download automatically.

**Use your own keys and never commit them to git or share them.** API calls cost a small amount;
the Claude method makes one call per item pair (n·(n−1)/2).

Get keys: [OpenAI](https://platform.openai.com/api-keys) · [Voyage](https://www.voyageai.com/) · [Anthropic](https://console.anthropic.com/)
