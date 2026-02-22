# LLM Lecture Notebooks

A series of hands-on Jupyter notebooks that guide you from foundational LLM infrastructure concepts through local inference, cloud APIs, multimodal AI, and Retrieval-Augmented Generation (RAG).

## Notebooks

| # | Notebook | Description |
|---|----------|-------------|
| 01 | [GPU VRAM & Model Feasibility](01_GPU_VRAM_Model_Feasibility_HFMem.ipynb) | Estimate GPU memory requirements for different model sizes and data types using `hf-mem`. |
| 02 | [Local LLM Inference with Ollama](02_Local_LLM_Inference_with_Ollama_Colab.ipynb) | Run open-source LLMs locally in Google Colab using Ollama with GPU support. |
| 03 | [Gemini API Basics](03_Gemini_API_Basics_Key_Setup_and_First_Prompts.ipynb) | Set up the Gemini API, craft your first prompts, and measure latency and token usage. |
| 04 | [Open vs Closed Models](04_Open_vs_Closed_Models_Gemini_vs_Local_Comparison.ipynb) | Benchmark Gemini against local Ollama models on quality, latency, cost, and privacy. |
| 05 | [Multimodal: Image Tagging & PDF Extraction](05_Multimodal_Comparison_Image_Tagging_and_PDF_Extraction.ipynb) | Use Gemini's multimodal capabilities for image captioning and structured PDF data extraction. |
| 06 | [RAG with In-Memory Vector DB](06_Gemini_API_RAG_InMemory_VectorDB.ipynb) | Build a complete RAG pipeline with Gemini embeddings and a Chroma in-memory vector database. |

## Prerequisites

- Python 3.10+
- A [Google AI Studio](https://aistudio.google.com/) API key (for notebooks 03–06)
- A CUDA-capable GPU is recommended for notebooks 01–02 (Google Colab T4 or better works well)

## Getting Started

1. Open any notebook in [Google Colab](https://colab.research.google.com/) or a local Jupyter environment.
2. Follow the setup cell at the top of each notebook to install dependencies.
3. For Gemini notebooks, store your API key as a Colab secret named `GEMINI_API_KEY` or set it as an environment variable.

## Learning Path

The series is designed to be followed in order:

```
Infrastructure        →  Local Inference  →  Cloud API  →  Advanced Capabilities
(01 VRAM estimation)     (02 Ollama)         (03 Gemini)   (04 Comparison)
                                                            (05 Multimodal)
                                                            (06 RAG)
```

## Key Tools & Libraries

| Library | Purpose |
|---------|---------|
| `hf-mem` | GPU VRAM estimation for HuggingFace models |
| `ollama` | Local LLM serving and inference |
| `google-genai` | Official Gemini API client |
| `chromadb` | In-memory vector database for RAG |
| `pillow` | Image loading and preprocessing |
| `pandas` | Data analysis and result comparison |

## License

See [LICENSE](LICENSE) for details.
