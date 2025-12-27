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

### LangGraph Deep Agents
**Platform:** LangChain AI  
**Status:** Modules 0-4 Completed (Course Completed)

A hands-on course focused on building deep agents capable of handling complex, long-running tasks. Implements advanced patterns including task planning, context offloading, and context isolation through sub-agent delegation.

### Deep Research
**Platform:** LangChain AI  
**Status:** Modules 1-5 Completed (Course Completed)

A comprehensive course on building production-ready deep research systems from scratch. Covers multi-phase research workflows including scoping, research execution, and report generation using advanced agent patterns and external tool integration.

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

### LangGraph Deep Agents

#### Module 0: Creating Agents
- **ReAct Agents:** Implemented Reasoning and Acting framework agents using create_agent abstraction
- **Tool Integration:** Built agents with calculator tools demonstrating tool calling and execution
- **State Management:** Extended AgentState with custom fields and reducer functions for state updates
- **Injected Parameters:** Used InjectedState and InjectedToolCallId to pass state and metadata to tools without LLM awareness
- **Command Updates:** Leveraged Command objects to update multiple state fields from tool returns
- **Key Takeaway:** The create_agent abstraction simplifies building production-ready ReAct agents with custom state management

#### Module 1: Task Planning with TODO Lists
- **DeepAgentState:** Extended state schema with todos list and files dictionary for comprehensive task tracking
- **TODO Structure:** Implemented structured tasks with content descriptions and status tracking (pending, in_progress, completed)
- **TODO Tools:** Created write_todos and read_todos tools for managing task lists within agent workflows
- **Context Rot Prevention:** Utilized continuous TODO list updates to maintain agent focus during long-running tasks with high tool call counts
- **Task Recitation:** Implemented pattern of rewriting TODO lists to keep objectives at end of context window
- **Key Takeaway:** Structured TODO lists enable agents to navigate complex multi-step tasks and prevent mission drift

#### Module 2: Virtual File Systems
- **Context Offloading:** Implemented filesystem operations to manage context window growth during complex tasks with high tool call counts
- **Virtual Filesystem:** Built dictionary-based mock filesystem within LangGraph state for thread-wise persistence
- **File Tools:** Created ls, read_file, and write_file tools for storing and retrieving information outside the context window
- **Strategic Storage:** Enabled agents to write token-heavy content to files and fetch information as needed rather than maintaining all data in context
- **Key Takeaway:** Context offloading through file systems prevents context accumulation while preserving access to critical information

#### Module 3: Context Isolation with Sub-agents
- **Sub-agent Delegation:** Implemented specialized sub-agents with isolated context windows to prevent context clashes and confusion
- **Sub-agent Registry:** Created registry system mapping subagent types to configured agents with specific tool sets and prompts
- **Task Tool:** Built delegation mechanism enabling parent agent to assign work to specialized sub-agents through task tool calls
- **Clean Separation:** Maintained isolation where sub-agents operate independently and return results to parent as ToolMessages
- **Key Takeaway:** Context isolation through sub-agent delegation enables focused task execution and prevents context pollution

#### Module 4: Complete Research Agent
- **Integration:** Combined TODO lists, file systems, and sub-agents into a fully functional deep research agent
- **Search Tool:** Implemented Tavily search with content offloading where full webpage content is saved to files and only summaries returned to agent
- **Content Processing:** Built pipeline for fetching webpage content, converting HTML to markdown, and generating structured summaries
- **Think Tool:** Created strategic reflection mechanism for agents to analyze findings and plan next research steps
- **Key Takeaway:** Deep agents combine task planning, context offloading, and context isolation to handle complex long-running research tasks

### Deep Research

#### Module 1: User Clarification and Brief Generation
- **User Clarification:** Implemented structured workflow to determine if additional context is needed from users before starting research
- **Brief Generation:** Transformed conversational user inputs into detailed research questions using Pydantic schemas
- **Structured Output:** Used ClarifyWithUser and ResearchQuestion schemas to prevent hallucination and ensure reliable decision making
- **LangGraph Commands:** Leveraged Command system for flow control and state updates across workflow phases
- **Conditional Routing:** Built two-step workflow with clarification phase followed by brief generation based on clarification needs
- **Key Takeaway:** Proper scoping through user clarification and structured brief generation ensures research addresses actual user intent

#### Module 2: Research Agent with Custom Tools
- **Agent Architecture:** Built iterative research agent using LLM decision node and tool execution node pattern
- **Sequential Tool Execution:** Implemented synchronous tool execution for reliability and simplicity
- **Search Integration:** Integrated Tavily search with content summarization to compress search results efficiently
- **Research Loop:** Created ReAct-style agent loop with conditional routing based on LLM decisions
- **Prompt Engineering:** Applied concrete heuristics including hard limits on tool calls and thinking tools to prevent excessive searching
- **Key Takeaway:** Research agents use flexible strategies guided by intermediate results to handle open-ended research tasks

#### Module 3: Research Agent with MCP
- **Model Context Protocol:** Integrated MCP servers as standardized tool access mechanism for research agents
- **MCP Architecture:** Implemented client-server communication using LangChain MCP Adapters for seamless integration
- **Filesystem Server:** Used Filesystem MCP Server providing file operations, directory management, and search capabilities
- **Async Tool Execution:** Implemented async-only operation required by MCP protocol for non-blocking concurrent operations
- **Protocol-Based Tools:** Leveraged MultiServerMCPClient for configuration-driven server setup and management
- **Key Takeaway:** MCP provides standardized protocol for AI tool access enabling integration of diverse tool ecosystems

#### Module 4: Research Supervisor
- **Supervisor Pattern:** Implemented coordination agent with worker agents for complex multi-topic research tasks
- **Parallel Research:** Built concurrent research execution using parallel tool calls to delegate independent sub-topics to sub-agents
- **Context Isolation:** Created separate context windows for different research topics to prevent context clash and confusion
- **Delegation Tools:** Developed structured tools (ConductResearch, ResearchComplete) for task assignment and completion
- **Scaling Rules:** Applied heuristics for determining when to use single agent versus multiple sub-agents based on request complexity
- **Key Takeaway:** Multi-agent coordination with context isolation enables handling complex research requests with multiple independent sub-topics

#### Module 5: Full Multi-Agent Research System
- **Three-Phase Architecture:** Integrated complete workflow combining scoping, multi-agent research, and report generation
- **System Integration:** Composed all previous components into end-to-end research system from user input to final report
- **State Management:** Implemented complex state flow across subgraphs with proper transitions between phases
- **Report Generation:** Added final synthesis phase to produce comprehensive research reports from aggregated findings
- **Thread Management:** Enabled conversation-based clarification with proper thread handling across workflow phases
- **Key Takeaway:** Complete research systems integrate scoping, coordinated execution, and synthesis to deliver production-ready deep research capabilities

## Technical Skills Acquired

- **Agent Frameworks:** LangChain, smolagents, and LangGraph for building AI agents
- **RAG Systems:** Vector databases, embeddings, and retrieval-augmented generation
- **Prompt Engineering:** Advanced templating, memory management, and output parsing
- **Tool Integration:** Custom tool development and multi-tool orchestration
- **Evaluation:** Automated and human evaluation methodologies for LLM applications
- **Long-Term Memory:** Memory stores, semantic and procedural memory management
- **Production Deployment:** Docker containerization, API integration, and deployment strategies
- **Task Planning:** TODO list management and structured task tracking for complex workflows
- **Context Management:** Context offloading through virtual file systems and context isolation through sub-agent delegation
- **Deep Agents:** Building production-ready agents capable of handling complex long-running tasks with advanced context engineering patterns
- **Research Systems:** Structured research workflows with scoping, clarification, and brief generation
- **Structured Output:** Pydantic schemas for reliable AI decision making and preventing hallucination
- **Multi-Agent Coordination:** Supervisor patterns and parallel research execution for complex multi-topic tasks
- **Protocol Integration:** Model Context Protocol (MCP) servers for standardized tool access and ecosystem integration

## Next Steps

This repository will continue to grow as I explore additional courses and frameworks in the Agentic AI space. Future areas of focus include:
- Advanced agent architectures and multi-agent systems
- Integration with other AI frameworks and tools
- Real-world application development and deployment