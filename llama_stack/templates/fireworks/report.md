# Report for fireworks distribution

## Supported Models
| Model Descriptor | fireworks |
|:---|:---|
| Llama-3-8B-Instruct | ❌ |
| Llama-3-70B-Instruct | ❌ |
| Llama3.1-8B-Instruct | ✅ |
| Llama3.1-70B-Instruct | ✅ |
| Llama3.1-405B-Instruct | ✅ |
| Llama3.2-1B-Instruct | ✅ |
| Llama3.2-3B-Instruct | ✅ |
| Llama3.2-11B-Vision-Instruct | ✅ |
| Llama3.2-90B-Vision-Instruct | ✅ |
| Llama3.3-70B-Instruct | ✅ |
| Llama-Guard-3-11B-Vision | ✅ |
| Llama-Guard-3-1B | ❌ |
| Llama-Guard-3-8B | ✅ |
| Llama-Guard-2-8B | ❌ |

## Inference
| Model | API | Capability | Test | Status |
|:----- |:-----|:-----|:-----|:-----|
| Llama-3.1-8B-Instruct | /chat_completion | streaming | test_text_chat_completion_streaming | ✅ |
| Llama-3.2-11B-Vision-Instruct | /chat_completion | streaming | test_image_chat_completion_streaming | ✅ |
| Llama-3.2-11B-Vision-Instruct | /chat_completion | non_streaming | test_image_chat_completion_non_streaming | ✅ |
| Llama-3.1-8B-Instruct | /chat_completion | non_streaming | test_text_chat_completion_non_streaming | ✅ |
| Llama-3.1-8B-Instruct | /chat_completion | tool_calling | test_text_chat_completion_with_tool_calling_and_streaming | ✅ |
| Llama-3.1-8B-Instruct | /chat_completion | tool_calling | test_text_chat_completion_with_tool_calling_and_non_streaming | ✅ |
| Llama-3.2-11B-Vision-Instruct | /chat_completion | log_probs | test_completion_log_probs_non_streaming | ✅ |
| Llama-3.2-11B-Vision-Instruct | /chat_completion | log_probs | test_completion_log_probs_streaming | ✅ |
| Llama-3.1-8B-Instruct | /completion | streaming | test_text_completion_streaming | ✅ |
| Llama-3.1-8B-Instruct | /completion | non_streaming | test_text_completion_non_streaming | ✅ |
| Llama-3.1-8B-Instruct | /completion | structured_output | test_text_completion_structured_output | ✅ |

## Vector IO
| Provider | API | Capability | Test | Status |
|:-----|:-----|:-----|:-----|:-----|
| inline::faiss | /retrieve |  | test_vector_db_retrieve | ✅ |

## Agents
| Provider | API | Capability | Test | Status |
|:-----|:-----|:-----|:-----|:-----|
| inline::meta-reference | /create_agent_turn | rag | test_rag_agent | ✅ |
| inline::meta-reference | /create_agent_turn | custom_tool | test_custom_tool | ✅ |
