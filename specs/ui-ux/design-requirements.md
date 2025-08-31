# UI/UX Design Requirements

## Design Philosophy

### Core Design Principles
1. **Natural**: Interface should feel like using a real notebook
2. **Focused**: Minimize distractions to encourage deep reflection
3. **Premium**: High-quality, polished experience worthy of paid app
4. **Accessible**: Usable by people with varying abilities
5. **Intentional**: Every design choice supports the journaling experience

### Visual Inspiration
- **GoodNotes**: Clean notebook metaphor, natural page interaction
- **Kings Journal**: Premium materials, masculine design aesthetic
- **MindJournal**: Supportive, warm color palette, clear typography
- **Apple Notes**: System integration, familiar iOS patterns

## Visual Design System

### Color Palette
```
Primary Colors:
- Deep Navy (#1B2951) - Trust, depth, premium feel
- Warm Gold (#D4AF37) - Growth, achievement, premium accent
- Sage Green (#87A96B) - Calm, mental health, balance

Supporting Colors:
- Light Cream (#FAF7F0) - Paper background, warmth
- Charcoal (#36454F) - Text, serious content
- Soft Blue (#7FB3D3) - Links, interactive elements

Semantic Colors:
- Success: Forest Green (#228B22)
- Warning: Amber (#FFC107)
- Error: Muted Red (#C5282F)
- Information: Ocean Blue (#0077BE)
```

### Typography
```
Primary Font: SF Pro (iOS system font)
- Display: SF Pro Display (headings, large text)
- Text: SF Pro Text (body content, UI elements)
- Rounded: SF Pro Rounded (friendly prompts, casual content)

Handwriting Font: Apple's handwriting recognition font
- Used for displaying converted handwritten text
- Maintains original character spacing and style
```

### Spacing and Layout
- **Base Unit**: 8pt grid system
- **Margins**: 16pt (small screens) to 24pt (large screens)
- **Content Width**: Max 680pt for readability
- **Touch Targets**: Minimum 44pt x 44pt
- **Card Radius**: 12pt for modern iOS feel

## Interface Structure

### Navigation Hierarchy
```
App Launch
├── Journal Library (main view)
│   ├── Journal Grid/List View
│   ├── Create New Journal
│   └── Settings/Profile
├── Journal Detail View
│   ├── Entry List (calendar/timeline)
│   ├── Search and Filter
│   └── Journal Settings
└── Entry Editor (writing canvas)
    ├── Drawing Canvas (PencilKit)
    ├── Template Prompts (overlay/sidebar)
    ├── Tool Palette
    └── Entry Actions (save, export, etc.)
```

### Screen Layouts

#### Journal Library
- **Header**: App title, user profile, settings icon
- **Main Content**: Grid of journal covers (2-3 columns on iPad)
- **Footer**: Create new journal FAB (Floating Action Button)
- **Secondary Actions**: Search, filter, sort options

#### Entry Editor (Primary Interface)
- **Full Screen Canvas**: Maximum writing space
- **Floating Tool Palette**: Minimalist, repositionable
- **Template Prompts**: Contextual overlay or collapsible sidebar
- **Navigation**: Subtle back button, entry navigation arrows
- **Status**: Auto-save indicator, sync status

## Interaction Design

### Apple Pencil Interactions
```
Pencil Gestures:
- Single tap: Select/focus
- Double tap: Switch tools (if supported)
- Scribble: Delete gesture for text
- Long press: Context menu
- Two-finger tap: Undo
- Three-finger tap: Redo
```

### Touch Interactions
```
Core Gestures:
- Tap: Select, activate
- Long press: Context menus, drag
- Pinch: Zoom in/out on canvas
- Pan: Navigate large pages
- Swipe: Page navigation, delete actions
```

### Keyboard Shortcuts (when connected)
```
Essential Shortcuts:
- Cmd+N: New entry
- Cmd+S: Manual save
- Cmd+Z: Undo
- Cmd+Shift+Z: Redo
- Cmd+F: Search
- Cmd+T: New journal
```

## Responsive Design

### iPad Orientations
- **Portrait**: Primary orientation for natural writing
- **Landscape**: Optimized layout with sidebar for templates
- **Split View**: Functional when using 1/3 or 2/3 screen space
- **Slide Over**: Basic functionality maintained

### Dynamic Type Support
- Support all iOS Dynamic Type sizes
- UI elements scale appropriately
- Maintain touch target minimums
- Text reflows properly in prompts

## Accessibility Requirements

### VoiceOver Support
- All interactive elements have clear labels
- Handwritten content has alt text from recognition
- Navigation order is logical and efficient
- Custom actions for complex gestures

### Motor Accessibility
- Alternative input methods for users who cannot handwrite
- Adjustable touch sensitivity
- Voice dictation support
- Switch control compatibility

### Visual Accessibility
- High contrast mode support
- Color blind friendly palette
- Reduce motion settings respected
- Clear visual hierarchy and focus indicators

## Animation and Transitions

### Micro-Interactions
- **Ink Rendering**: Smooth, natural ink flow
- **Page Turns**: Realistic page flip animation
- **Tool Selection**: Subtle highlight and feedback
- **Button Presses**: Gentle scale and shadow
- **Loading States**: Meaningful progress indicators

### Navigation Transitions
- **Push/Pop**: Standard iOS navigation
- **Modal Present**: Scale transition for templates
- **Tab Changes**: Cross-fade for different journals
- **Search**: Smooth reveal/hide of search interface

### Performance Guidelines
- All animations 60fps on supported devices
- Reduce motion preferences respected
- No animation longer than 0.5 seconds
- Meaningful loading states for operations >1 second

## Content Guidelines

### Template Design Standards
- Clear, engaging prompt questions
- Appropriate white space for responses
- Visual hierarchy with headers and subheadings
- Consistent formatting across template family
- Cultural sensitivity in language and imagery

### Prompt Writing Guidelines
- Questions should be open-ended but focused
- Avoid leading or biased language
- Include context or examples when helpful
- Vary question types (reflection, planning, gratitude)
- Professional review for mental health content

## Error States and Empty States

### Error Handling
- Clear, actionable error messages
- Graceful degradation when features unavailable
- Retry mechanisms for network issues
- Help documentation easily accessible

### Empty States
- Inspiring messages for new users
- Clear next steps and calls to action
- Visual examples of filled journals
- Easy template discovery and selection