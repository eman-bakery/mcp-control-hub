# AGENTS.md

## Project overview
This repository is for MCP Control Hub, a mobile-first web platform and remote MCP server for connecting internal tools and third-party services to AI agents.

## Stack direction
- TypeScript first
- Mobile-first UI
- Cloudflare-compatible deployment
- Modular connector architecture
- OAuth where needed
- No hardcoded secrets

## Architecture rules
- Keep connectors isolated as separate modules.
- Keep UI separate from server logic.
- Keep auth logic separate from connector logic.
- Prefer reusable abstractions over platform-specific hacks.
- Design for future connectors from day one.

## UI rules
- Mobile-first layouts only
- Clean modern dashboard style
- Touch-friendly controls
- Minimal friction for connecting services
- Clear status indicators for each connector

## Security rules
- Never commit secrets
- Use environment variables for credentials
- Use least-privilege scopes
- Log connector actions safely
- Keep auditability in mind

## Code rules
- Use clear folder names
- Use descriptive function names
- Avoid unnecessary complexity
- Prefer maintainable structure over clever shortcuts
- Document any important architectural decision

## Current phase
We are in the foundation stage:
1. Define project structure
2. Create core folders
3. Add initial docs
4. Build the first MCP server shell
5. Add connectors one by one
6. Add the dashboard UI

