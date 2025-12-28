# Agentic AI Strands Projects

A collection of AI agent implementations using the Strands framework for building intelligent, autonomous systems with knowledge management and external API integration capabilities.

## Project Overview

This repository contains practical implementations of agentic AI systems that can:
- Store and retrieve information from knowledge bases
- Make intelligent decisions about data operations
- Integrate with external APIs for real-time data
- Process natural language queries and commands

## Components

### 1. Knowledge Base System (`knowledge_base.py`)
Core infrastructure for creating and managing AWS Bedrock knowledge bases with OpenSearch integration.

**Features:**
- Amazon Bedrock knowledge base creation
- OpenSearch vector database setup
- Titan embedding model integration (v2:0)
- Automated resource provisioning


### 2. Knowledge Base Agent (`knowledge_base_agent.py`)
Intelligent agent that automatically determines whether to store or retrieve information based on user queries.

![Screenshot 2025-12-27 091806.png](https://images.tomarkdown.dev/uploaded/lj9qgfew0248r1n5.png)

**Capabilities:**
- Natural language understanding for intent detection
- Automatic store/retrieve decision making
- Clean, user-friendly interactions
- Memory persistence across sessions

**Example Usage:**
```python
# Store information
"Remember that my birthday is on July 25"

# Retrieve information  
"When is my birthday?"
```

### 3. Weather Agent (`weather_agentcore.py`)
HTTP-enabled agent that fetches real-time weather data from the National Weather Service API.
![Screenshot 2025-12-27 091728.png](https://images.tomarkdown.dev/uploaded/j4raqrm3oifupuwx.png)

**Features:**
- Multi-step API workflows (coordinates → forecast)
- Error handling for HTTP requests
- Natural language weather queries
- Real-time data processing

## Quick Start

### Prerequisites
```bash
pip install strands-agents boto3 opensearch-py retrying
```

### Environment Setup
```bash
# AWS credentials required
export AWS_ACCESS_KEY_ID=<your-key>
export AWS_SECRET_ACCESS_KEY=<your-secret>
export AWS_DEFAULT_REGION=us-east-1
```

### Running the Agents

1. **Knowledge Base Agent:**
```bash
python knowledge_base_agent.py
```

2. **Weather Agent:**
```bash
python weather_agentcore.py
```

3. **Knowledge Base Setup:**
```bash
python knowledge_base.py
```

## Architecture

```
User Query → Agent → Decision Logic → Action (Store/Retrieve/API Call) → Response
```

The agents use the Strands framework to:
1. Parse natural language input
2. Determine appropriate actions
3. Execute operations (knowledge base or API calls)
4. Return formatted responses

## Configuration

### Knowledge Base Settings
- Embedding Model: `amazon.titan-embed-text-v2:0`
- Vector Dimensions: 1024
- Backend: OpenSearch Serverless

### Supported Operations
- **Store**: Save information to knowledge base
- **Retrieve**: Query stored information
- **Weather**: Get current weather conditions
- **Forecast**: Retrieve weather predictions

## Error Handling

The agents include robust error handling for:
- AWS service connectivity issues
- API rate limiting
- Invalid queries
- Network timeouts
- Authentication failures

## Development

### Adding New Capabilities
1. Extend the agent's tool set
2. Implement new decision logic
3. Add error handling
4. Test with various query types

### Customization
- Modify embedding models in `knowledge_base.py`
- Adjust vector dimensions for different models
- Add new API integrations following the weather agent pattern

## Troubleshooting

**Common Issues:**
- **Knowledge base not found**: Ensure AWS credentials are configured
- **API timeouts**: Check network connectivity and API limits
- **Embedding errors**: Verify model availability in your region

**Debug Mode:**
```bash
export STRANDS_DEBUG=1
python <agent_script>.py
```
