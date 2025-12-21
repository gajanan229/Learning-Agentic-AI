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

### LangGraph Essentials
**Platform:** DeepLearning.AI  
**Status:** Completed

A concise refresher course covering core LangGraph concepts. Taken to reinforce fundamentals before continuing with the more advanced LangChain Academy course.

### Introduction to LangGraph - LangChain Academy
**Platform:** [LangChain Academy](https://academy.langchain.com/courses/intro-to-langgraph)  
**Status:** Completed

A comprehensive 6-module course providing deep dive training into LangGraph fundamentals, covering state management, human-in-the-loop patterns, long-term memory, and production deployment strategies.

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

### LangGraph Essentials

#### Lesson 1: States & Nodes
- **Graph Structure:** Defined shared state using TypedDict and created node functions
- **Key Takeaway:** Nodes are functions that transform state within a graph workflow

#### Lesson 2: Parallel Execution
- **Concurrent Nodes:** Implemented parallel execution with multiple outgoing edges
- **State Reducers:** Used operator.add to accumulate results from parallel branches
- **Key Takeaway:** LangGraph handles parallel execution automatically when nodes have multiple edges

#### Lesson 3-4: Conditional Edges & Memory
- **Dynamic Routing:** Built conditional edges using Command objects and routing functions
- **State Persistence:** Implemented memory with checkpointers for state management
- **Key Takeaway:** Conditional logic enables intelligent workflow branching based on state

#### Lesson 5: Human-in-the-Loop
- **Interrupt Function:** Paused execution for human approval using interrupt()
- **Checkpointing:** Saved state between pauses to resume workflows
- **Key Takeaway:** Interrupts enable human oversight for critical decision points

#### Lesson 6: Email Workflow Agent
- **Integrated Workflow:** Built a complete email processing agent combining all concepts
- **Key Takeaway:** LangGraph components compose into production-ready applications

### Introduction to LangGraph - LangChain Academy

#### Module 1: Simple Graph, Chain & Router
- **Simple Graph:** Built basic LangGraph with nodes, edges, and conditional routing using TypedDict state
- **Chain:** Implemented chat model integration with message state, tool binding, and tool execution workflows
- **Router:** Created intelligent routing between direct responses and tool calls using conditional edges and ToolNode
- **Key Takeaway:** LangGraph provides foundational building blocks for workflow orchestration

#### Module 2: State Management
- **State Schema:** Mastered multiple state definition approaches including TypedDict, Dataclasses, and Pydantic models for structured data validation
- **State Reducers:** Implemented reducer functions to handle concurrent state updates and branching workflows using Annotated types and operator functions
- **Key Takeaway:** Flexible state management enables complex data flow patterns

#### Module 3: Human-in-the-Loop
- **Streaming:** Implemented multiple streaming modes to visualize graph output and chat model tokens during execution
- **Breakpoints:** Used interrupt_before and interrupt_after to pause execution for human approval workflows
- **State Editing:** Modified graph state and injected human feedback during interrupted execution
- **Dynamic Breakpoints:** Implemented conditional interrupts using NodeInterrupt based on runtime logic
- **Time Travel:** Replayed and forked from past states for debugging and alternative execution paths
- **Key Takeaway:** Human-in-the-loop patterns enable oversight and intervention in agent workflows

#### Module 4: Multi-Agent Workflows
- **Parallelization:** Implemented fan-out and fan-in patterns for concurrent node execution with state reducers
- **Sub-graphs:** Created modular multi-agent systems with separate state spaces communicating through overlapping keys
- **Map-Reduce:** Built workflows that distribute tasks across parallel nodes and aggregate results
- **Research Assistant:** Developed a complete multi-agent research system with planning, multi-turn interviews, and report generation
- **Key Takeaway:** Multi-agent architectures enable complex problem decomposition and parallel processing

#### Module 5: Long-Term Memory
- **Memory Store:** Introduced LangGraph Memory Store for saving and retrieving long-term memories across threads
- **Profile Schema:** Saved semantic memories to a structured user profile using Trustcall for schema updates
- **Collection Schema:** Saved memories to collections instead of single profiles for managing multiple items
- **Memory Agent:** Built task_mAIstro, an agent with long-term memory managing ToDo lists with both semantic and procedural memory
- **Key Takeaway:** Long-term memory enables personalized and context-aware agent interactions

#### Module 6: Production Deployment
- **Creating Deployment:** Used LangGraph CLI to build Docker images and create self-hosted deployments
- **Connecting to Deployment:** Interacted with deployed agents using LangGraph API endpoints for Runs, Threads, and Store
- **Assistants:** Created and versioned assistants for experimentation and different use cases
- **Double Texting:** Handled concurrent user messages gracefully using rejection and enqueuing strategies
- **Key Takeaway:** LangGraph Platform provides production-ready deployment and management capabilities

## Technical Skills Acquired

- **Agent Frameworks:** LangChain, smolagents, and LangGraph for building AI agents
- **RAG Systems:** Vector databases, embeddings, and retrieval-augmented generation
- **Prompt Engineering:** Advanced templating, memory management, and output parsing
- **Tool Integration:** Custom tool development and multi-tool orchestration
- **Evaluation:** Automated and human evaluation methodologies for LLM applications
- **Long-Term Memory:** Memory stores, semantic and procedural memory management
- **Production Deployment:** Docker containerization, API integration, and deployment strategies

## Next Steps

This repository will continue to grow as I explore additional courses and frameworks in the Agentic AI space. Future areas of focus include:
- Advanced agent architectures and multi-agent systems
- Integration with other AI frameworks and tools
- Real-world application development and deployment