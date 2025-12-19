# AI Agents Workshop - Build Intelligent AI Agents with Amazon Bedrock & Strands

This repository contains materials from the AI For Bharat Workshop 4, focusing on building intelligent AI agents using Amazon Bedrock and the Strands SDK. The workshop provides comprehensive tutorials, samples, and a complete personal assistant project implementation.

## 📁 Repository Structure

```
├── 01 tutorial/           # Step-by-step learning materials
├── 02 samples/           # Practical implementation examples  
├── Blog-Personal assistant project/  # Complete personal assistant implementation
└── README.md            # This file
```

## 🎯 Workshop Overview

Learn to build sophisticated AI agents that can:
- Interact with AWS services (Bedrock, DynamoDB, Knowledge Base)
- Use multiple AI models (OpenAI GPT, Ollama, Amazon Bedrock)
- Implement multi-agent collaboration patterns
- Deploy to AWS infrastructure (Lambda, Fargate)
- Handle real-world tasks like calendar management

## 📚 Tutorial Content

### **01 Tutorial** - Fundamentals & Advanced Concepts

**Fundamentals:**
- F1: Creating your first Strands agent
- F2: Model providers (OpenAI, Ollama)
- F3: AWS services integration
- F4: Tools (MCP tools, custom tools)
- F5: Streaming responses
- F6: Bedrock Guardrail integration
- F7: Memory and persistent agents
- F8: Observability and evaluation

**Multi-Agent Systems:**
- M1: Agent as tool pattern
- M2: Swarm agent architecture
- M3: Graph agent networks

**Deployment:**
- D1: AWS Lambda deployment
- D2: AWS Fargate deployment

### **02 Samples** - Real-World Applications

- **Restaurant Assistant**: Booking and management system
- **Personal Assistant**: Calendar and task management

## 🤖 Personal Assistant Project

The `Blog-Personal assistant project` folder contains a complete implementation showcasing:

### Features
- **Calendar Management**: Create, update, list appointments
- **Multi-Agent Architecture**: Specialized agents working together
- **AWS Integration**: Bedrock models and AWS services
- **Interactive CLI**: User-friendly command interface

### Quick Start
```bash
cd "Blog-Personal assistant project"
pip install -r requirements.txt
python calendar_assistant.py
```

### Architecture
The personal assistant uses a multi-agent pattern where specialized agents handle different domains:
- Calendar Agent: Appointment management
- Main Coordinator: User interaction and task routing

## 🛠️ Prerequisites

- Python 3.8+
- AWS Account with Bedrock access
- AWS CLI configured
- Basic understanding of AI/ML concepts

## 📋 Setup Instructions

1. **Clone the repository**
```bash
git clone <repository-url>
cd "workshop 4 Build intelligent AI agents with Amazon Bedrock & Strands"
```

2. **Set up Python environment**
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
```

3. **Configure AWS credentials**
```bash
aws configure
# OR set environment variables
export AWS_ACCESS_KEY_ID=your_access_key
export AWS_SECRET_ACCESS_KEY=your_secret_key
export AWS_DEFAULT_REGION=us-east-1
```

4. **Install dependencies** (in each project folder)
```bash
pip install -r requirements.txt
```

## 🚀 Getting Started

1. **Start with Fundamentals**: Begin with `01 tutorial/01 fundamentals/01-first-agent`
2. **Explore Samples**: Try the examples in `02 samples/`
3. **Build Your Own**: Use the personal assistant as a template for your projects

## 🔧 Key Technologies

- **Strands SDK**: Agent framework and orchestration
- **Amazon Bedrock**: Foundation models and AI services
- **AWS Services**: Lambda, Fargate, DynamoDB, Knowledge Base
- **Python**: Primary development language
- **MCP (Model Context Protocol)**: Tool integration standard

## 📖 Learning Path

1. **Beginner**: Start with F1-F4 tutorials
2. **Intermediate**: Complete F5-F8 and try samples
3. **Advanced**: Implement multi-agent systems (M1-M3)
4. **Production**: Deploy using D1-D2 patterns

## 🤝 Workshop Context

This repository was created for **AI For Bharat Workshop 4**, demonstrating practical AI agent development using AWS services. The materials progress from basic concepts to production-ready implementations.

## 📝 Additional Resources

- [Strands Documentation](https://strandsagents.com/)
- [Amazon Bedrock User Guide](https://docs.aws.amazon.com/bedrock/)
- [AWS CLI Documentation](https://docs.aws.amazon.com/cli/)

## 🎉 Next Steps

After completing this workshop:
- Build your own specialized agents
- Integrate with your existing AWS infrastructure  
- Explore advanced multi-agent patterns
- Deploy to production environments

---

**Happy Building strands agent!** 🚀✨
