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

### LangChain for LLM Application Development

#### Lesson 1: Models, Prompts and Output Parsers
- **LangChain Abstraction:** Simplified model interactions and prompt templating
- **Output Parsers:** Built structured data extraction from LLM responses
- **Key Takeaway:** LangChain reduces boilerplate while maintaining prompt engineering flexibility

#### Lesson 2: Memory for LLMs
- **Memory Types:** Implemented buffer, window, token-based, and summary memory systems
- **Key Takeaway:** Memory management enables coherent long-running dialogues within token limits

#### Lesson 3: Chains
- **Chain Types:** Built sequential and router chains for complex workflows
- **Key Takeaway:** Chains compose simple operations into powerful multi-step applications

#### Lesson 4: Question Answering over Documents
- **RAG Implementation:** Combined document retrieval with LLM generation
- **Key Takeaway:** RAG enables accurate domain-specific answers using proprietary data

#### Lesson 5: Evaluation
- **Evaluation Methods:** Implemented manual and LLM-assisted evaluation systems
- **Key Takeaway:** Systematic evaluation is essential for reliable applications

#### Lesson 6: Agents
- **Agent Architecture:** Built reasoning systems with tool selection and custom integrations
- **Key Takeaway:** Agents enable autonomous AI systems that reason and take actions

### Hugging Face AI Agents Course

#### Unit 1: Introduction to Agents
- **Agent Architecture:** Agents combine LLM reasoning with tool usage in Think-Act-Observe cycles
- **smolagents Framework:** Built functional agents with tool integration and proper message formatting
- **Key Takeaway:** Agents extend LLMs beyond text generation through structured decision-making

#### Unit 2.1: The smolagents Framework
- **Agent Types:** Mastered CodeAgents and ToolCallingAgents for different use cases
- **Multi-Agent Systems:** Orchestrated specialized agents for complex problem-solving
- **Key Takeaway:** smolagents enables sophisticated workflows through modular design

#### Unit 2.3: The LangGraph Framework
- **Graph Architecture:** Built stateful workflows using nodes, edges, and conditional branching
- **State Management:** Implemented persistent state across workflow steps
- **Key Takeaway:** LangGraph provides precise control for production-ready agent applications

#### Unit 3: Use Case for Agentic RAG
- **Custom RAG Tools:** Built specialized retrieval systems with intelligent tool selection
- **Real-World Application:** Created Alfred, a gala host agent with multi-tool integration
- **Key Takeaway:** Agentic RAG enables autonomous information retrieval from multiple sources

## Technical Skills Acquired

- **Agent Frameworks:** LangChain, smolagents, and LangGraph for building AI agents
- **RAG Systems:** Vector databases, embeddings, and retrieval-augmented generation
- **Prompt Engineering:** Advanced templating, memory management, and output parsing
- **Tool Integration:** Custom tool development and multi-tool orchestration
- **Evaluation:** Automated and human evaluation methodologies for LLM applications

## Next in Learning Path

### Introduction to LangGraph - LangChain Academy
**Platform:** [LangChain Academy](https://academy.langchain.com/courses/intro-to-langgraph)  
**Status:** In Progress - Module 1 Completed, Module 2 Started

This comprehensive 6-module course provides deep dive training into LangGraph fundamentals, covering state management, human-in-the-loop patterns, long-term memory, and production deployment strategies.

#### Module 1 Completed:
- **Simple Graph:** Built basic LangGraph with nodes, edges, and conditional routing using TypedDict state
- **Chain:** Implemented chat model integration with message state, tool binding, and tool execution workflows  
- **Router:** Created intelligent routing between direct responses and tool calls using conditional edges and ToolNode

#### Module 2 Progress:
- **State Schema:** Mastered multiple state definition approaches including TypedDict, Dataclasses, and Pydantic models for structured data validation
- **State Reducers:** Implemented reducer functions to handle concurrent state updates and branching workflows using Annotated types and operator functions

## Next Steps

This repository will continue to grow as I explore additional courses and frameworks in the Agentic AI space. Future areas of focus include:
- Advanced agent architectures and multi-agent systems
- Integration with other AI frameworks and tools
- Real-world application development and deployment