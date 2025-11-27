# CLAUDE.md - AI Assistant Guide for Interceptor

## Project Overview

**Interceptor** is a 2D top-down arcade game inspired by Spy Hunter with a Mad Max post-apocalyptic theme. This is a learning project focused on:
- Understanding GitHub workflows and version control
- Improving Python coding skills
- Mobile development using iPhone as the primary development platform
- Game development with Pygame

**Author:** Ryan
**Started:** July 15th, 2024
**Primary Language:** Python
**Game Framework:** Pygame
**Development Platform:** iPhone (using GitHub and CodeSandBox)

## Repository Structure

```
Interceptor/
├── src/                    # Source code directory
│   └── main.py            # Main game entry point (currently empty)
├── assets/                # Game assets (images, sounds, etc.)
│   └── placeholder.txt    # Placeholder for asset organization
├── README.md              # Project documentation
└── CLAUDE.md             # This file - AI assistant guide
```

## Development Context

### Current State
- **Early Stage:** The project is in initial setup phase
- **main.py:** Currently empty, awaiting game implementation
- **Assets:** Not yet populated
- **Target Platform:** The game is being developed on iPhone, which may influence tooling choices

### Technology Stack
- **Language:** Python 3.x
- **Framework:** Pygame (for 2D game rendering and game loop)
- **Version Control:** Git/GitHub
- **Development Environment:** Mobile-friendly (CodeSandBox, GitHub on iPhone)

## AI Assistant Guidelines

### When Working on This Project

1. **Understand the Learning Context**
   - This is a learning project for someone new to GitHub and game development
   - Provide clear explanations for code changes
   - Prioritize simple, readable solutions over complex optimizations
   - Add helpful comments to explain game development concepts

2. **Code Style Conventions**
   - Use Python PEP 8 style guide
   - Clear, descriptive variable names (e.g., `player_car`, `enemy_vehicles`, `score`)
   - Add docstrings to classes and non-trivial functions
   - Keep functions small and focused on single responsibilities

3. **Game Development Patterns**
   - Follow standard Pygame structure:
     - Initialization (pygame.init())
     - Game loop (event handling, update, render)
     - Clean shutdown
   - Separate concerns: game logic, rendering, input handling
   - Consider creating classes for: Player, Enemy, Weapon, PowerUp, GameState

4. **File Organization Suggestions**
   ```
   src/
   ├── main.py              # Game entry point and main loop
   ├── player.py            # Player car class
   ├── enemy.py             # Enemy vehicle classes
   ├── weapon.py            # Weapon systems
   ├── powerup.py           # Power-up items
   ├── config.py            # Game configuration (screen size, colors, etc.)
   └── utils.py             # Utility functions

   assets/
   ├── images/              # Sprites and graphics
   ├── sounds/              # Sound effects and music
   └── fonts/               # Game fonts
   ```

5. **Dependencies Management**
   - Create a `requirements.txt` file listing dependencies:
     ```
     pygame>=2.0.0
     ```
   - Consider mobile-friendly libraries that work well in limited environments

6. **Testing Approach**
   - Due to mobile development constraints, focus on:
     - Manual testing workflows
     - Simple unit tests for game logic (separate from rendering)
     - Clear instructions for running/testing on different platforms

### Git Workflow

1. **Branch Naming**
   - Feature branches: `feature/description`
   - Bug fixes: `fix/description`
   - Claude AI branches: `claude/claude-md-*` (auto-generated)

2. **Commit Messages**
   - Use clear, descriptive messages
   - Format: `<type>: <description>`
   - Types: `feat`, `fix`, `docs`, `refactor`, `test`, `asset`
   - Examples:
     - `feat: add player car movement controls`
     - `fix: resolve collision detection bug`
     - `asset: add Mad Max themed car sprites`
     - `docs: update README with installation steps`

3. **Commit Scope**
   - Keep commits focused on single features or fixes
   - Don't mix refactoring with new features
   - Commit working code (game should run without errors)

### Common Tasks

#### Starting Game Development
1. Read existing code in `src/main.py`
2. Set up basic Pygame window and game loop
3. Implement player controls
4. Add enemies and collision detection
5. Implement scoring system
6. Add weapons and power-ups

#### Adding New Features
1. Consider mobile development constraints
2. Keep code simple and well-commented
3. Test manually (describe test steps in commit message)
4. Update README if user-facing changes

#### Working with Assets
1. Place images in `assets/images/`
2. Place sounds in `assets/sounds/`
3. Use placeholder graphics for prototyping
4. Document asset requirements in comments
5. Consider asset size for mobile performance

#### Debugging Assistance
1. Add print statements for debugging (mobile-friendly)
2. Check Pygame initialization and display setup
3. Verify file paths for assets (case-sensitive on Linux/Mac)
4. Test on desktop Python if mobile environment has issues

### Mad Max Theme Guidelines

When implementing game features, keep the theme in mind:
- **Visual Style:** Post-apocalyptic, rugged, desert wasteland
- **Vehicles:** Armored, weaponized, makeshift modifications
- **Color Palette:** Browns, oranges, grays, rust tones
- **Enemies:** Varied vehicle types (motorcycles, trucks, war rigs)
- **Weapons:** Machine guns, missiles, mines, oil slicks
- **Environment:** Desert roads, rocks, debris, destroyed infrastructure

### Mobile Development Considerations

Since this is developed on iPhone:
1. **File Paths:** Use relative paths, test on multiple platforms
2. **Performance:** Keep sprite counts reasonable, optimize rendering
3. **Controls:** Design for both keyboard (testing) and touch (future mobile port)
4. **Asset Sizes:** Compress images, use appropriate resolutions
5. **Code Complexity:** Favor clarity over complex optimizations
6. **Testing:** Provide clear instructions for running in mobile environments

### Code Review Checklist

Before committing, verify:
- [ ] Code follows PEP 8 style guidelines
- [ ] Functions and classes have docstrings
- [ ] No hardcoded file paths (use os.path.join)
- [ ] Game runs without errors
- [ ] New features are commented and explained
- [ ] Assets are properly referenced
- [ ] README updated if needed
- [ ] Commit message is clear and descriptive

### Resources and References

- **Pygame Documentation:** https://www.pygame.org/docs/
- **Python PEP 8:** https://pep8.org/
- **Spy Hunter Gameplay:** Classic arcade mechanics for reference
- **Mad Max Theme:** Visual and thematic inspiration

### Questions to Ask Before Implementation

1. Does this feature align with the learning goals?
2. Is the solution simple enough for a beginner to understand?
3. Will this work in a mobile development environment?
4. Have I explained the "why" behind code decisions?
5. Is the Mad Max theme maintained?

### Project Goals Priority

1. **Learning GitHub:** Clear commits, branching, version control
2. **Learning Python:** Clean, readable, well-structured code
3. **Learning Game Development:** Basic game loops, sprites, collision detection
4. **Mobile Adaptation:** Successfully developing on iPhone
5. **Fun Gameplay:** Engaging Mad Max themed arcade experience

## Quick Start for AI Assistants

When first engaging with this project:

1. Check current state of `src/main.py`
2. Review recent commits to understand progress
3. Ask user about specific goals for this session
4. Propose implementation plan before coding
5. Provide clear explanations with code changes
6. Test changes (or provide testing instructions)
7. Commit with descriptive messages

## Notes

- This is an **active learning project** - prioritize educational value
- The developer is working on **iPhone** - consider mobile constraints
- **Simplicity over complexity** - this is for learning, not production
- **Document everything** - help the developer learn as they go
- **Encourage best practices** - but explain why they matter

---

Last Updated: 2025-11-27
