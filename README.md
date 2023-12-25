# ADL-Final Project
Final Project for ADL

## Directory Structure
```shell
.
├── Taiwan-LLM-7B-v2.0-chat
├── adapter_model
├── chat_rag.py
├── data
│   ├── preprocessed
│   │   └── speech
│   ├── speech
│   ├── test
│   └── test_result
├── embedding.py
├── inference.py
└── speech.ipynb
```
## File Discription
- Folder `Taiwan-LLM-7B-v2.0-chat` is used to put Taiwan-LLama model.
- Folder `adapter_model` is used to put weights that we fine tune Taiwan-LLama model by qLora.
- Folder `data` is used to put all data we used.
  - Folder `preprocessed` is used to put preprocessed data.
  - Folder `speech` is used to put raw data we obtain from <https://hackmd.io/@johnshao>.
  - Folder `test` is used to put test data that we separate from training data.
  - Folder `test_result` is used to put preprocessed test data.
- chat_rag.py is used to construct a demo web.
- embedding.py is used to create a vector database using data in `./data/preprocessed/speech`.



