# AWS Bedrock Workshop 1 - AI for Bharat  

A comprehensive workshop for learning AWS Bedrock capabilities including text generation, image processing, embeddings, RAG, and more.

## Project Structure

```
workshop 1 bedrock/
├── code/workshop/           # Main workshop code
│   ├── completed/          # Complete implementations
│   ├── labs/              # Lab exercises
│   ├── data/              # Workshop data and embeddings
│   └── LICENSE            # MIT License
└── sample_images/         # Sample images for testing
```

## Features

### Text & Language Models
- **API Integration** - Basic Bedrock API usage
- **Text Generation** - Simple text completion
- **Streaming** - Real-time text streaming
- **Chatbot** - Interactive conversation interface
- **Multimodal Chatbot** - Text and image conversations
- **JSON Processing** - Structured data handling
- **CSV Analysis** - Data processing workflows
- **Summarization** - Document summarization
- **Temperature Control** - Model parameter tuning

### Image Processing
- **Image Generation** - Text-to-image creation
- **Image Understanding** - Visual content analysis
- **Image Variation** - Style and content variations
- **Image Extension** - Outpainting capabilities
- **Image Insertion** - Inpainting features
- **Image Masking** - Selective editing
- **Image Replacement** - Object replacement
- **Image Background** - Background modification
- **Image Style Mixing** - Style transfer
- **Image Search** - Visual similarity search

### Advanced Features
- **Embeddings** - Vector representations
- **RAG (Retrieval Augmented Generation)** - Knowledge-enhanced responses
- **Guardrails** - Content safety and filtering
- **Tool Use** - Function calling capabilities
- **Prompt Engineering** - Advanced prompting techniques
- **Recommendations** - Content recommendation system

## Quick Start

1. **Prerequisites**
   - AWS CLI configured
   - Python 3.x installed
   - Required Python packages (boto3, streamlit, etc.)

2. **Run Examples**
   ```bash
   cd code/workshop/completed/api
   python bedrock_api.py
   ```

3. **Start Streamlit Apps**
   ```bash
   streamlit run code/workshop/completed/chatbot/chatbot_app.py
   ```

## Workshop Structure

- **Labs** - Hands-on exercises with starter code
- **Completed** - Full implementations for reference
- **Data** - Pre-processed embeddings and sample datasets

## Sample Images

The `sample_images/` directory contains test images for image processing labs including desk scenes, various objects, and example images for different use cases.

## License

MIT No Attribution - See LICENSE file for details.

Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.

