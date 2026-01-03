
# Metadata

**Title**: Company Knowledge Graph – Core Definition
**Owner**: Pranav Pandey
**Version**: 1.0.0
**Type**: Article
**Created Date**: 21 Dec 2025
**Last Updated**: 21 Dec 2025


# Content

### Overview

The main idea of this system is to build a company-wide knowledge graph that the company can fully rely on. This knowledge graph will act as the single source of truth for the organization.

All company content will be created from this knowledge graph. All decisions, processes, and actions taken by the company will be derived from the knowledge stored within it.

The knowledge graph is designed to be collaborative. Anyone in the company can create nodes, update existing nodes, and contribute to the graph.

This document exists to explain what the knowledge graph is, how it works, and how it will be built.

### Knowledge Graph Structure

The knowledge graph is composed of two core components:

#### Nodes

Nodes represent entities in the system. A node can represent anything, including but not limited to:

- A concept
- An article
- A person
- A process
- A document
- Any other unit of knowledge

Each node is a self-contained unit of information.

#### Edges

Edges represent connections between nodes. A connection simply means that two nodes are related in some meaningful way. These connections allow knowledge to be linked, explored, and reused across the graph.

### Node Structure

Every node in the knowledge graph must follow a fixed structure consisting of four parts.

#### 1. Title

- A short, clear description of the node
- Maximum length: 160 characters

#### 2. Metadata

Metadata defines the identity and lifecycle of the node.

- Title: The title of the document
- Owner: Owner of the document
- Version: The version of the document will be updated when we will update the document. It has a format replace.major.minor so anytime you do any of the respective update you will update the version
- Type (Text, Web Link, YouTube Video, Image, Article)
- Created Date
- Last Updated

#### 3. Content

The Content section stores the actual knowledge of the node.

- This is where all internal information is written
- It contains explanations, definitions, processes, and decisions
- Main nodes must never contain direct references to external entities

This section is the authoritative source for the information represented by the node.

#### 4. References

The References section is used to connect the node to other nodes in the knowledge graph.

- References may only point to internal nodes
- External sources must never be referenced directly

### Node Types

Nodes are organized into two categories.

#### Main Nodes

Main nodes contain the core internal knowledge of the company.

- They store original, company-owned content
- They never directly reference external sources
- If an external source is needed, a reference node must be created first

#### Reference Nodes

Reference nodes are special nodes used to represent external sources.

- Their content consists of external links or external material
- They act as a bridge between internal knowledge and external information

Main nodes may reference reference nodes, but never external sources directly.

  

### Tools and Storage
- Obsidian will be used to create, manage, and visualize the knowledge graph
- Git will be used for version control, change tracking, and cloud storage of all nodes

# References

[[Obsidian]]
