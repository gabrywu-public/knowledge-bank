# Knowledge Bank

An intelligent knowledge management system for Claude Code that automatically captures, stores, and retrieves development knowledge during your coding sessions.

## Overview

Knowledge Bank is a lightweight Claude Code plugin that transforms your development workflow by:

- 🧠 **Automatically capturing** valuable development insights through Claude Code's hook system
- 📚 **Storing knowledge** in a local SQLite database with powerful full-text search
- 🔍 **Smart retrieval** of relevant context during development sessions
- 🏗️ **Intelligent organization** using multi-dimensional classification
- ⚡ **Zero-friction integration** with your existing Claude Code workflow

## Installation

### Prerequisites

- Node.js >= 18.0.0
- Claude Code CLI installed and configured

### Quick Setup

```bash
# Install Knowledge Bank globally
npm install -g @gabrywu/knowledge-bank --registry https://registry.npmjs.org
# For alpha/beta versions, use:
npm install -g @gabrywu/knowledge-bank@alpha --registry https://registry.npmjs.org

# Install the Knowledge Bank plugin
knowledge-bank install

# Uninstall plugin
knowledge-bank uninstall
```

### Verification

```bash
# Check installation status
knowledge-bank knowledge-status
```

## Web Interface

Knowledge Bank includes a built-in web interface for browsing and exploring your local knowledge database through a user-friendly dashboard.

### Starting the Web Interface

```bash
# Start web server (production mode)
knowledge-bank web
```

The web interface will be available at `http://localhost:3000` (or your specified port).

### Features

The web interface provides comprehensive access to your knowledge database:

#### 🏠 **Dashboard Overview**
- **System Statistics**: Quick overview of repositories, sessions, knowledge items, and hook events
- **Repository Browser**: Navigate through your Git repositories and their associated knowledge
- **Real-time Data**: Live view of your current knowledge database state

#### 📊 **Knowledge Management**
- **Knowledge Items Viewer**: Browse, search, and filter all captured knowledge items
  - Filter by type (architecture, code_pattern, tool_usage, config, pitfall, API_usage, exploration)
  - Filter by status (draft, suggested, verified)
  - Filter by scope (personal, project, organization)
  - Full-text search across titles, summaries, and content
- **Markdown Rendering**: Rich display of knowledge content with proper formatting
- **Knowledge Details**: Expandable rows showing complete knowledge item information

#### 📝 **Session Management**
- **Session History**: View all Claude Code sessions organized by repository
- **Session Details**: Browse session metadata including working directory, branch, and timestamps
- **Session Filtering**: Search sessions by session ID, branch, or working directory

#### 🪝 **Hook Event Tracking**
- **Event History**: Monitor all Claude Code hook events across sessions
- **Event Filtering**: Filter by event name, session ID, or repository
- **Event Timeline**: Chronological view of hook activations and system events

#### 🗄️ **Database Browser**
- **Table Explorer**: Direct access to all database tables (repository, session, knowledge_item, hook_event)
- **Schema Viewer**: Inspect database structure and relationships
- **Advanced Filtering**: Multiple filter options per table with pagination
- **Sortable Columns**: Click headers to sort by any column (ascending/descending)

#### 🔍 **Advanced Search & Navigation**
- **Cross-table Relationships**: Navigate between related repositories, sessions, and knowledge items
- **Repository-centric View**: See all sessions, knowledge, and events for each repository
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Real-time Updates**: Reflects the latest database state on page refresh

The web interface transforms your local knowledge database into an accessible, browsable resource that helps you leverage your accumulated development experience effectively.

## License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

---

Transform your development workflow with intelligent knowledge management. Get started with Knowledge Bank today!