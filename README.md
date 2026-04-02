# LANGGRAPH
In this module we will learn in depth about LangGraph framework and how it is revolutionizing the development of ai agents. This course is taught by Nitesh and the link to the courses are provided below.  
- [LangGraph Playlist](https://www.youtube.com/watch?v=yC36gN-rqjo&list=PLKnIA16_RmvYsvB8qkUQuJmJNuiCUJFPL&index=2)

## What is LangGraph?  
LangGraph is an orchestration framework for building **intelligent**, **stateful** and **multi-step LLM workflows**. It enabales advanced features like **parallelism**, **loops**, **branching**, **memory**, and, **resumability** making it ideal for Agentic Application. It models your logic as a **graph of nodes**(tasks) and **edges**(routing) instead of a linear chain.  

```mermaid
graph TD
    A[User Input] --> B[LLM]
    B --> C{Has tool call?}
    C -->|Yes| D[Tool Execution]
    D --> B
    C -->|No| E[Final Answer]

    style A fill:#4CAF50,color:#fff
    style B fill:#2196F3,color:#fff
    style C fill:#FF9800,color:#fff
    style D fill:#9C27B0,color:#fff
    style E fill:#F44336,color:#fff

    linkStyle 0 stroke:#4CAF50,stroke-width:2px
    linkStyle 1 stroke:#2196F3,stroke-width:2px
    linkStyle 2 stroke:#F44336,stroke-width:2px
    linkStyle 3 stroke:#9C27B0,stroke-width:2px
    linkStyle 4 stroke:#4CAF50,stroke-width:2px
```