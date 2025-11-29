# Full Stack Chat Platform

This project provides a complete chat platform that integrates PocketBase for user management and data storage, Ollama for language model inference, and Svelte for the frontend interface. The application supports simultaneous conversations with multiple AI models and includes comprehensive chat management features.

## Technology Stack

- **Frontend**: Svelte with TypeScript
- **Backend Runtime**: Bun (Node.js compatible)
- **Database & Auth**: PocketBase
- **AI Models**: Ollama integration
- **Build System**: Vite
- **Styling**: Pico CSS

## Prerequisites

- Bun runtime (or Node.js as alternative)
- Ollama server with at least one model installed (e.g., llama3, gemma)
- Linux environment (for included PocketBase binary)

## Installation & Setup

```bash
# Install dependencies
bun install

# Start PocketBase database server
bun run pocketbase

# Start development server
bun run dev

# Build for production
bun run build

# Preview production build
bun run preview
```

## Service Configuration

- Application: http://localhost:1337
- PocketBase: http://localhost:8090
- Ollama: http://localhost:11434
- PocketBase Admin UI: http://localhost:1337/_/

The development server automatically proxies requests to both PocketBase and Ollama services.

## Features

### User Management
- Complete authentication system via PocketBase
- Support for OAuth providers (Google, GitHub, etc.)
- User session management

### Chat System
- Create and manage multiple chat conversations
- Simultaneous queries to multiple AI models
- Real-time streaming responses
- Model switching during conversations
- Chat history persistence

### Interface
- Multiple layout modes including compact view
- Auto-resizing message input
- Live markdown rendering of AI responses
- Automatic chat scrolling
- Dark mode support

### Technical Features
- Double Enter keypress for message sending
- Local storage for user preferences
- TypeScript throughout the codebase
- ESLint and Prettier configuration

## Project Structure

```
src/ - Application source code
pb/ - PocketBase server and configuration
static/ - Static assets
tests/ - Test suites
```

## Development Notes

This project was developed over approximately 30-40 hours as part of a full-stack web development course at JKU Linz. The implementation includes no prior experience with SvelteKit or PocketBase, demonstrating a rapid learning and development cycle.

## License

Creative Commons Zero v1.0 Universal - You are free to use, modify, and distribute this code for any purpose.
