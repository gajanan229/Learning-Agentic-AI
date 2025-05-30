# Learning Agentic AI

This repository documents my journey learning Agentic AI and building intelligent applications using Large Language Models (LLMs). The focus is on practical implementations using modern frameworks and understanding how AI agents can be designed to reason, act, and interact with various tools and data sources.

## Course Completed

### LangChain for LLM Application Development
**Instructors:** Harrison Chase (Co-Founder and CEO at LangChain) & Andrew Ng (Founder of DeepLearning.AI)  
**Platform:** DeepLearning.AI  
**Duration:** 1 hour intensive course

This course provided hands-on experience with the LangChain framework, covering essential patterns for building robust LLM applications beyond simple API calls.

## Key Learnings by Lesson

### Lesson 1: Models, Prompts and Output Parsers
**Core Concepts:** Understanding the foundation of LLM application development
- **Direct API Integration:** Learned to make direct calls to OpenAI's API and handle responses
- **LangChain Abstraction:** Discovered how LangChain simplifies model interactions through standardized interfaces
- **Prompt Templates:** Implemented reusable prompt templates for consistent formatting and variable injection
- **Output Parsers:** Built structured data extraction from LLM responses, converting unstructured text into JSON objects
- **Key Takeaway:** LangChain's abstraction layer significantly reduces boilerplate code while maintaining flexibility for complex prompt engineering

### Lesson 2: Memory for LLMs
**Core Concepts:** Managing conversation state and context limitations
- **ConversationBufferMemory:** Implemented basic conversation history storage for maintaining context across interactions
- **ConversationBufferWindowMemory:** Learned to manage memory by keeping only the most recent exchanges to control token usage
- **ConversationTokenBufferMemory:** Explored token-based memory management for more precise control over context size
- **ConversationSummaryMemory:** Implemented automatic conversation summarization to maintain context while reducing token consumption
- **Key Takeaway:** Memory management is crucial for building conversational applications that can maintain coherent, long-running dialogues while respecting token limits

### Lesson 3: Chains
**Core Concepts:** Creating sequences of LLM operations for complex workflows
- **LLMChain:** Built basic chains that combine prompts with models for single-step operations
- **SimpleSequentialChain:** Implemented linear workflows where the output of one chain becomes the input of the next
- **SequentialChain:** Created more complex workflows with multiple inputs and outputs, allowing for branching logic
- **Router Chain:** Developed intelligent routing systems that can direct inputs to different specialized chains based on content
- **Key Takeaway:** Chains enable the creation of sophisticated applications by composing simple LLM operations into powerful workflows

### Lesson 4: Question Answering over Documents
**Core Concepts:** Building knowledge-based applications using proprietary data
- **Document Loading:** Learned to ingest and process various document formats (CSV, text, PDFs)
- **Vector Stores:** Implemented document embeddings and similarity search using DocArrayInMemorySearch
- **Retrieval-Augmented Generation (RAG):** Built systems that combine document retrieval with LLM generation for accurate, contextual answers
- **RetrievalQA Chains:** Created end-to-end Q&A systems that can query large document collections
- **Key Takeaway:** RAG patterns enable LLMs to provide accurate, up-to-date answers about specific domains by grounding responses in retrieved documents

### Lesson 5: Evaluation
**Core Concepts:** Measuring and improving LLM application performance
- **Test Data Generation:** Learned strategies for creating comprehensive test datasets for LLM applications
- **Manual Evaluation:** Implemented human-in-the-loop evaluation processes for quality assessment
- **LLM-Assisted Evaluation:** Built systems where LLMs evaluate other LLM outputs, enabling scalable assessment
- **Automated Testing Pipelines:** Created frameworks for continuous evaluation of application performance
- **Key Takeaway:** Systematic evaluation is essential for building reliable LLM applications, requiring both automated metrics and human judgment

### Lesson 6: Agents
**Core Concepts:** Building reasoning systems that can use tools and make decisions
- **Built-in Tools:** Integrated existing tools like Wikipedia search, mathematical computation, and web search
- **Custom Tool Creation:** Developed domain-specific tools and integrated them into agent workflows
- **Agent Types:** Explored different reasoning patterns including zero-shot React agents and conversational agents
- **Tool Selection Logic:** Implemented systems where agents can intelligently choose which tools to use based on the task
- **Key Takeaway:** Agents represent the evolution toward more autonomous AI systems that can reason about problems and take actions using available tools

## Technical Skills Acquired

- **LangChain Framework:** Comprehensive understanding of components, chains, and agent patterns
- **Vector Databases:** Experience with embedding-based search and retrieval systems
- **Prompt Engineering:** Advanced techniques for crafting effective prompts and handling edge cases
- **Memory Management:** Strategies for maintaining conversation state while optimizing token usage
- **Tool Integration:** Building and integrating custom tools for specialized agent capabilities
- **Evaluation Methodologies:** Both automated and human evaluation approaches for LLM applications

## Next Steps

This repository will continue to grow as I explore additional courses and frameworks in the Agentic AI space. Future areas of focus include:
- Advanced agent architectures and multi-agent systems
- Integration with other AI frameworks and tools
- Real-world application development and deployment
- Performance optimization and scaling strategies