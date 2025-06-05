# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Structure

This is a single-file HTML project (`shooting_2025_06_06.html`) containing a complete Japanese shooting game built with vanilla JavaScript and HTML5 Canvas.

## Architecture

- **Single HTML file**: Contains all HTML structure, CSS styling, and JavaScript game logic
- **Canvas-based game**: Uses HTML5 Canvas with 2D context for rendering
- **Responsive design**: Adapts canvas size for mobile devices (< 500px width)
- **Touch controls**: Automatic touch button display for mobile devices
- **SVG assets**: Player, enemy, and bullet sprites are embedded as SVG data URIs

## Key Game Components

- **Player**: Blue triangle spaceship at bottom of screen
- **Enemies**: Red oval enemies spawning from top
- **Bullets**: Yellow projectiles fired by player
- **Game states**: Start screen, playing, paused, game over
- **Progressive difficulty**: Enemy speed and spawn rate increase with level

## Development Commands

Since this is a single HTML file with no build process:
- **Run game**: Open `shooting_2025_06_06.html` in any modern web browser
- **Edit**: Modify the HTML file directly (all code is embedded)

## Code Organization within the File

1. **CSS styles** (lines 9-137): Game UI and responsive layout
2. **HTML structure** (lines 139-166): Canvas, controls, and UI elements  
3. **JavaScript game logic** (lines 168-543):
   - DOM element references
   - Game variables and configuration
   - SVG asset definitions
   - Event listeners
   - Core game functions (movement, collision, spawning)
   - Game loop and rendering
   - Mobile touch controls
   - Window resize handling

## Game Configuration

Key gameplay variables are defined around lines 188-225:
- Canvas dimensions
- Player/enemy/bullet sizes and speeds
- Spawn intervals and timing
- Score and level progression

## Mobile Support

The game automatically detects touch devices and shows touch controls. Canvas resizes to fit mobile screens while maintaining playability.