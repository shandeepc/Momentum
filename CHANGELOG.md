# Changelog

All notable changes to this project will be documented here.

## v2.0.0 (2026-07-14)

### Added
- **Multi-Selection & Playing-Card Fan Drag (`Ctrl` / `Meta` + Drag)**: Select and drag multiple tasks simultaneously without releasing the `Ctrl` key. Dragged cards display as a realistic playing-card fan pinched at the bottom-left corner (`transform-origin: 12% 88%`) with a `+N` stack counter badge.
- **Custom Color-Coded Labels & Tag Filtering**: Assign pre-defined or dynamically created tags to tasks with unique color coding. Filter tasks instantly from the toolbar tag filter dropdown.
- **Board Insights & Analytics Dashboard**: Interactive analytics panel showcasing task completion rates, productivity progress, and breakdowns by priority, status, and tag.
- **Card Cover Accents & Custom Color Highlights**: Personalize task cards with custom header color accent strips and highlights.
- **Unified Custom UI Dropdown System (`CustomSelect`)**: Upgraded all toolbar and modal `<select>` elements to custom div-based overlay dropdowns with auto-refresh (`MutationObserver`) synchronization.

### Changed & Fixed
- **Drag & Drop Engine Overhaul**: Eliminated dragging glitches and column drop-zone flickering, improved visual hover states, and refined auto-scrolling when dragging near top/bottom screen edges.
- **Multi-Drag Clone & Selection Preservation**: Fixed multi-drag stack visibility by ensuring cloned items reset inline display properties before original cards are hidden.
- **Sort & DOM Order Normalization**: Automatic transition to manual sort mode when reordering cards manually, ensuring persistent index ordering across LocalStorage.

## v1.0.0 (2026-07-10)

### Added
- Kanban board
- Drag & Drop
- Yet To Start / In Progress / Completed columns
- Subtasks
- Overall Progress Bar
- Search
- Filters
- Sorting
- Archive & Restore
- Export / Import JSON
- Dark Mode
- Keyboard Shortcuts
- Offline LocalStorage
- Responsive UI
