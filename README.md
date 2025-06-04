# Learning Agentic AI

This repository documents my journey learning Agentic AI and building intelligent applications using Large Language Models (LLMs). The focus is on practical implementations using modern frameworks and understanding how AI agents can be designed to reason, act, and interact with various tools and data sources.

## Courses Completed

### LangChain for LLM Application Development
**Instructors:** Harrison Chase (Co-Founder and CEO at LangChain) & Andrew Ng (Founder of DeepLearning.AI)  
**Platform:** DeepLearning.AI  
**Duration:** 1 hour intensive course

This course provided hands-on experience with the LangChain framework, covering essential patterns for building robust LLM applications beyond simple API calls.

### Hugging Face AI Agents Course
**Instructors:** Joffrey Thomas, Ben Burtenshaw, Thomas Simonini & Sergio Paniego (Hugging Face Team)  
**Platform:** [Hugging Face Learn](https://huggingface.co/learn/agents-course/unit1)  
**Status:** Units 1, 2.1, 2.3, and 3 Completed (Course Paused)

This comprehensive course provided hands-on experience with multiple AI agent frameworks and real-world implementations. Covered foundational agent concepts, advanced frameworks (smolagents, LangGraph), and practical Agentic RAG applications through the creation of Alfred, a sophisticated gala host agent.

## Key Learnings by Lesson

### LangChain Course

#### Lesson 1: Models, Prompts and Output Parsers
**Core Concepts:** Understanding the foundation of LLM application development
- **Direct API Integration:** Made direct calls to OpenAI's API and handled responses
- **LangChain Abstraction:** Simplified model interactions through standardized interfaces
- **Prompt Templates:** Implemented reusable templates for consistent formatting and variable injection
- **Output Parsers:** Built structured data extraction from LLM responses to JSON objects
- **Key Takeaway:** LangChain reduces boilerplate code while maintaining flexibility for complex prompt engineering

#### Lesson 2: Memory for LLMs
**Core Concepts:** Managing conversation state and context limitations
- **ConversationBufferMemory:** Basic conversation history storage for maintaining context
- **ConversationBufferWindowMemory:** Managed memory by keeping recent exchanges to control token usage
- **ConversationTokenBufferMemory:** Token-based memory management for precise context control
- **ConversationSummaryMemory:** Automatic conversation summarization to maintain context while reducing tokens
- **Key Takeaway:** Memory management is crucial for coherent, long-running dialogues while respecting token limits

#### Lesson 3: Chains
**Core Concepts:** Creating sequences of LLM operations for complex workflows
- **LLMChain:** Basic chains combining prompts with models for single-step operations
- **SimpleSequentialChain:** Linear workflows where output becomes input for the next step
- **SequentialChain:** Complex workflows with multiple inputs/outputs and branching logic
- **Router Chain:** Intelligent routing systems directing inputs to specialized chains based on content
- **Key Takeaway:** Chains enable sophisticated applications by composing simple LLM operations into powerful workflows

#### Lesson 4: Question Answering over Documents
**Core Concepts:** Building knowledge-based applications using proprietary data
- **Document Loading:** Ingested and processed various document formats (CSV, text, PDFs)
- **Vector Stores:** Implemented document embeddings and similarity search using DocArrayInMemorySearch
- **Retrieval-Augmented Generation (RAG):** Combined document retrieval with LLM generation for accurate answers
- **RetrievalQA Chains:** Created end-to-end Q&A systems for querying large document collections
- **Key Takeaway:** RAG patterns enable accurate, domain-specific answers by grounding responses in retrieved documents

#### Lesson 5: Evaluation
**Core Concepts:** Measuring and improving LLM application performance
- **Test Data Generation:** Created comprehensive test datasets for LLM applications
- **Manual Evaluation:** Implemented human-in-the-loop evaluation processes
- **LLM-Assisted Evaluation:** Built systems where LLMs evaluate other LLM outputs for scalable assessment
- **Automated Testing Pipelines:** Created frameworks for continuous evaluation
- **Key Takeaway:** Systematic evaluation is essential for reliable LLM applications, requiring both automated metrics and human judgment

#### Lesson 6: Agents
**Core Concepts:** Building reasoning systems that can use tools and make decisions
- **Built-in Tools:** Integrated existing tools like Wikipedia search, mathematical computation, and web search
- **Custom Tool Creation:** Developed domain-specific tools and integrated them into agent workflows
- **Agent Types:** Explored different reasoning patterns including zero-shot React agents and conversational agents
- **Tool Selection Logic:** Implemented systems for intelligent tool selection based on task requirements
- **Key Takeaway:** Agents represent evolution toward autonomous AI systems that can reason and take actions using available tools

### Hugging Face AI Agents Course

#### Unit 1: Introduction to Agents
**Core Concepts:** Foundational understanding of AI Agents and their components

- **Agent Architecture:** Learned that agents consist of an LLM "brain" that interprets instructions, reasons about problems, and decides which tools to use for task completion
- **LLM Fundamentals:** Understood autoregressive token prediction, special tokens (EOS, chat delimiters), and the transformer architecture's attention mechanism
- **Chat Templates & Messages:** Implemented proper message formatting using system/user/assistant roles and model-specific special tokens for conversation flow
- **Think-Act-Observe Cycle:** Mastered the core agent workflow where agents reason about problems, take actions using tools, and observe results to inform next steps
- **Tool Integration:** Built custom tools using the @tool decorator and integrated external capabilities like timezone lookup and web search
- **smolagents Framework:** Created functional agents using Hugging Face's smolagents library with proper tool registration and prompt templates

**Key Takeaway:** Agents extend LLM capabilities beyond text generation by combining reasoning, tool usage, and environmental interaction in a structured decision-making loop

#### Unit 2.1: The smolagents Framework
**Core Concepts:** Advanced agent architectures and production-ready implementations

- **CodeAgents vs ToolCallingAgents:** Mastered both code-generating agents that write Python snippets and JSON-based tool calling patterns for different use cases
- **Advanced Tool Development:** Built sophisticated tools with proper type hints, error handling, and documentation for complex workflows
- **Multi-Agent Systems:** Orchestrated multiple specialized agents to solve complex tasks like Batman filming location analysis with cargo plane calculations
- **Vision Agents:** Integrated Vision-Language Models for image processing, character identification, and multimodal reasoning tasks
- **Production Patterns:** Implemented robust error handling, fallback mechanisms, and scalable agent architectures for real-world deployment

**Key Takeaway:** smolagents enables sophisticated agent workflows through modular design, supporting both code execution and tool calling paradigms for complex problem-solving

#### Unit 2.3: The LangGraph Framework
**Core Concepts:** Production-ready agent workflows with graph-based state management

- **Graph Architecture:** Mastered StateGraph fundamentals where nodes are Python functions performing work and edges control workflow direction with conditional branching
- **State Management:** Implemented centralized state objects that persist across nodes, enabling complex workflows like email processing with spam detection and response generation
- **Workflow Control:** Built sophisticated agent loops with conditional edges, enabling dynamic routing based on state conditions and supporting both linear and cyclic execution patterns
- **Vision Integration:** Developed multimodal agents combining document analysis, OCR text extraction, and LLM reasoning for comprehensive document processing workflows

**Key Takeaway:** LangGraph provides precise control over agent execution through graph-based workflows, enabling production-ready applications with complex state management and conditional logic

#### Unit 3: Use Case for Agentic RAG
**Core Concepts:** Real-world implementation of intelligent knowledge retrieval systems

- **Custom RAG Tools:** Built specialized retrieval tools using BM25Retriever for guest information lookup with Document objects and metadata management
- **Agentic Decision Making:** Implemented agents that intelligently choose when to use RAG vs other tools (web search, weather APIs) based on query context
- **Real-World Use Case:** Created Alfred, a sophisticated gala host agent managing guest relations, weather monitoring, and event coordination through multiple integrated tools

**Key Takeaway:** Agentic RAG enables intelligent knowledge systems where agents autonomously decide how to retrieve and combine information from multiple sources for complex real-world scenarios

## Technical Skills Acquired

- **LangChain Framework:** Comprehensive understanding of components, chains, and agent patterns
- **Vector Databases:** Experience with embedding-based search and retrieval systems
- **Prompt Engineering:** Advanced techniques for crafting effective prompts and handling edge cases
- **Memory Management:** Strategies for maintaining conversation state while optimizing token usage
- **Tool Integration:** Building and integrating custom tools for specialized agent capabilities
- **Evaluation Methodologies:** Both automated and human evaluation approaches for LLM applications
- **smolagents Framework:** Hands-on experience with Hugging Face's agent development toolkit
- **Chat Templates:** Understanding of message formatting and special tokens across different LLM architectures

## Next in Learning Path

### Introduction to LangGraph - LangChain Academy
**Platform:** [LangChain Academy](https://academy.langchain.com/courses/intro-to-langgraph)  
**Status:** Enrolled - Starting Soon

This comprehensive 6-module course provides deep dive training into LangGraph fundamentals, covering state management, human-in-the-loop patterns, long-term memory, and production deployment strategies.

## Next Steps

This repository will continue to grow as I explore additional courses and frameworks in the Agentic AI space. Future areas of focus include:
- Advanced agent architectures and multi-agent systems
- Integration with other AI frameworks and tools
- Real-world application development and deployment