# LHI Browser Automation Dashboard

A unified browser automation control center for managing Puppeteer, Playwright, and Kapture MCPs with intelligent Chrome profile management.

## 🚧 Status: Planning Phase

This module is currently in the planning phase. See [PLANNING.md](./PLANNING.md) for strategic planning details and [TASK.md](./TASK.md) for progress tracking.

## Overview

The LHI Browser Automation Dashboard provides a centralized web-based interface for:
- Managing browser automation across multiple MCP implementations
- Consistent Chrome profile selection and management
- Script recording, conversion, and playback
- Real-time monitoring of automation tasks
- Cross-platform support (Mac and Linux)

## Architecture

Built with:
- **Frontend**: React + LHI UI Framework (emotion CSS-in-JS)
- **Core**: Modular LHI node modules
- **Integration**: MCP bridges for Puppeteer, Playwright, and Kapture
- **Storage**: Local JSON configuration with ~/.lhi/browser-config.json

## Key Features (Planned)

### Profile Management
- Unified Chrome profile selection across all MCPs
- Visual profile selector with avatar display
- Persistent profile configuration
- Multi-browser support preparation

### Browser Automation Cards
- **Puppeteer Card**: Integration with lhi_puppeteer_browser
- **Playwright Card**: New LHI-Playwright wrapper
- **Kapture Card**: Browser tab management integration

### Script Management
- Universal script format (JSON-based)
- Script conversion between MCP formats
- Recording and playback capabilities
- Script library with categorization

### Monitoring
- Real-time status updates
- Console output monitoring
- Error tracking and debugging
- Performance metrics

## Development Phases

### Planning (Current Phase)
1. **Phase 1**: Research & Documentation Retrieval ✅
2. **Phase 2**: Architecture Design ⏳
3. **Phase 3**: Refinement & Validation
4. **Phase 4**: Pre-Implementation Planning

### Implementation (Upcoming)
1. Foundation & UI Shell
2. Core Components
3. Service Integration
4. Functionality Implementation
5. Polish & Testing

## Module Structure

```
lhi_browser_automation_dashboard/
├── .docs/              # Documentation library
│   ├── planning/       # Planning phase documents
│   ├── dependencies/   # Dependency documentation
│   └── architecture/   # Architecture diagrams
├── src/                # Source code (to be created)
├── scripts/            # Build and utility scripts
├── PLANNING.md         # Strategic planning
├── TASK.md            # Task tracking
└── README.md          # This file
```

## Dependencies

### LHI Modules
- `lhi_chrome_profile_utils` - Chrome profile selection
- `lhi_ui_framework` - UI components and styling
- `lhi_puppeteer_browser` - Existing automation infrastructure

### External (Research in Progress)
- React
- Emotion CSS-in-JS
- MCP Protocol clients

## Installation

*Installation instructions will be added after implementation phase begins.*

## Usage

*Usage documentation will be added after implementation phase begins.*

## Development

### Prerequisites
- Node.js 18+
- Chrome/Chromium browser
- LHI Scripts environment configured

### Setup
```bash
# Clone if not already present
cd $LHI_SCRIPTS_ROOT/lhi_modules/lhi_git_projects/LifeHackInnovationsLLC/lhi_node_modules/
git clone [repository-url] lhi_browser_automation_dashboard

# Install dependencies (when available)
cd lhi_browser_automation_dashboard
npm install
```

### Running Development Server
*Development server instructions will be added after implementation begins.*

## Contributing

This module follows LHI development standards:
- UI-first development approach
- Comprehensive documentation at each phase
- Modular, reusable components
- Cross-platform compatibility

## License

MIT - Life Hack Innovations LLC

## Contact

For questions or support, contact Life Hack Innovations LLC.

---

*Module Type: web-app*  
*Form Factor: lhi_node_modules*  
*Created: 2025-01-09*