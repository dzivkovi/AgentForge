## **Models YAML Documentation**

### **Overview**

The `models.yaml` file is dedicated to configurations related to Large Language Models (LLM). It encompasses model settings, available models, and a list of default parameters.

### **Formatting Guidelines**

- This file is organized into sections, each representing specific aspects of model configurations.
- Parameters can be overridden by individual agents, as outlined in the [**Overriding Default Configurations Documentation**](Overrides/OverridingConfig.md).

### **Sample Configuration**

```yaml
EmbeddingLibrary:
  library: sentence_transformers

ModelLibrary:
  claude: claude-2
  fast_model: gpt-3.5-turbo-0613
  smart_model: gpt-4

ModelSettings:
  API: openai_api
  Model: fast_model
  Params:
    max_new_tokens: 2000
    temperature: 0.5
    top_p: 0.1
    n: 1
    stop: null
    do_sample: true
    return_prompt: false
    return_metadata: false
    typical_p: 0.95
    repetition_penalty: 1.05
    encoder_repetition_penalty: 1.0
    top_k: 40
    min_length: 10
    no_repeat_ngram_size: 0
    num_beams: 1
    penalty_alpha: 0
    length_penalty: 1
    early_stopping: false
    pad_token_id: null
    eos_token_id: null
    use_cache: true
    num_return_sequences: 1
    bad_words_ids: null
    seed: -1
```

---
