# Safety Document Navigator

**Industry:** Energy

**Repository:** [tekvo-ai-hub/energy-safety-rag](https://github.com/tekvo-ai-hub/energy-safety-rag)

## Description
On-device assistant for retrieving field safety procedures from documents.

## Requirements
### Functional
- Support document search by voice/text.
- Index field guides.
- Offline access to emergency protocols.
### Non-Functional
- Runs on rugged tablets.
- No internet required.
- Fast response.
## Solution Design
**LLM:** TinyLlama
**Vector DB:** FAISS

### Components
- Voice/Text Input
- Doc Preprocessor
- Vector Search Engine
- LLM Responder
### Data Flow
$ Text → Chunk → Embed → FAISS → Retrieve → Prompt → LLM

### Tech Stack
- **Frontend:** Qt
- **Backend:** C++ + Python
- **Storage:** SQLite
- **Deployment:** Edge Binary
