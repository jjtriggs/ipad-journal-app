# User Stories and Use Cases

## Epic 1: Core Journaling Experience

### User Story 1.1: Natural Handwriting
**As a** user who loves handwriting  
**I want** to write naturally with my Apple Pencil  
**So that** journaling feels as satisfying as pen and paper  

**Acceptance Criteria:**
- Apple Pencil input has <20ms latency
- Pressure sensitivity affects line thickness
- Multiple pen styles available (ballpoint, marker, pencil)
- Palm rejection works perfectly
- Can write at any angle on the page

### User Story 1.2: Guided Prompts
**As a** person seeking personal growth  
**I want** structured questions that guide my reflection  
**So that** I can make meaningful progress on my goals  

**Acceptance Criteria:**
- Daily prompts appear automatically
- Prompts are categorized (productivity, mental health, gratitude)
- Can skip prompts that don't resonate
- Prompts adapt based on previous responses
- Clear instructions for each prompt type

### User Story 1.3: Template Selection
**As a** user with specific journaling goals  
**I want** to choose from different journal template styles  
**So that** my journaling experience matches my intentions  

**Acceptance Criteria:**
- Template library with preview images
- Categories: Daily Reflection, Goal Setting, Gratitude, Mental Health
- Can switch templates between entries
- Templates include both layout and prompt structure
- Free templates available, premium templates clearly marked

## Epic 2: Organization and Navigation

### User Story 2.1: Multiple Journals
**As a** user with different life areas to track  
**I want** to maintain separate journals for different purposes  
**So that** I can organize my thoughts appropriately  

**Acceptance Criteria:**
- Create unlimited journals with custom names
- Each journal can have different template defaults
- Visual journal covers/thumbnails
- Easy switching between journals
- Archive/delete journals when needed

### User Story 2.2: Entry Management
**As a** regular journal user  
**I want** to easily find and organize my past entries  
**So that** I can track my progress and revisit insights  

**Acceptance Criteria:**
- Calendar view of all entries
- Search through handwritten text
- Tag entries with custom labels
- Filter by date, journal, or tags
- Bookmark important entries

## Epic 3: Apple Pencil Integration

### User Story 3.1: Advanced Pen Features
**As a** creative journaler  
**I want** full control over my writing tools  
**So that** I can express myself visually as well as textually  

**Acceptance Criteria:**
- Pressure sensitivity controls line weight
- Tilt detection for shading effects
- Double-tap Apple Pencil to switch tools
- Eraser functionality (tip vs barrel)
- Undo/redo with Apple Pencil gestures

### User Story 3.2: Handwriting Recognition
**As a** user who wants to find specific content  
**I want** my handwriting automatically converted to searchable text  
**So that** I can quickly locate past insights  

**Acceptance Criteria:**
- Real-time handwriting recognition
- 90%+ accuracy for legible handwriting
- Search works across all entries
- Can copy recognized text to other apps
- Option to disable for privacy

## Epic 4: Cloud and Sync

### User Story 4.1: Cross-Device Access
**As a** user with multiple Apple devices  
**I want** my journals synced across all my devices  
**So that** I can journal wherever I am  

**Acceptance Criteria:**
- iCloud sync across iPad, iPhone, Mac
- Offline writing with sync when connected
- Conflict resolution for simultaneous edits
- Sync status clearly indicated
- Full journal history preserved

### User Story 4.2: Backup and Export
**As a** user investing time in journaling  
**I want** to ensure my entries are safe and exportable  
**So that** I never lose my personal growth journey  

**Acceptance Criteria:**
- Automatic cloud backup of all entries
- Export individual entries as PDF/image
- Export entire journals with formatting preserved
- Import from other journaling apps
- Local backup options

## Epic 5: Premium Features and Monetization

### User Story 5.1: Template Store
**As a** user wanting specialized journaling approaches  
**I want** access to expert-designed templates  
**So that** I can explore new methods for personal growth  

**Acceptance Criteria:**
- Browse template store by category
- Preview templates before purchase
- One-click purchase and download
- Templates include instructions and examples
- Regular new template releases

### User Story 5.2: Advanced Analytics
**As a** premium user tracking personal growth  
**I want** insights into my journaling patterns and progress  
**So that** I can see measurable improvement over time  

**Acceptance Criteria:**
- Writing frequency and word count trends
- Mood tracking from journal sentiment
- Goal completion tracking
- Habit formation insights
- Progress sharing options

## Use Cases

### Primary Use Case: Daily Reflection Journal
1. User opens app at end of day
2. Today's prompt automatically appears
3. User reads prompt: "What challenged you most today and how did you handle it?"
4. User writes 1-2 paragraphs with Apple Pencil
5. App recognizes handwriting for future search
6. Entry auto-saves to current journal
7. User sets reminder for tomorrow

### Secondary Use Case: Goal Planning Session
1. User creates new journal: "2024 Goals"
2. Selects "Goal Setting" template
3. Template provides structured prompts for 90-day planning
4. User writes goals using combination of text and diagrams
5. Template includes check-in prompts for weekly review
6. User bookmarks key insights for easy reference

### Tertiary Use Case: Mental Health Check-in
1. User feeling overwhelmed opens mental health template
2. Guided prompts help identify specific stressors
3. Template includes coping strategy suggestions
4. User writes through emotions with supportive prompts
5. Optional mood tracking integration
6. Entries can be shared with therapist (export feature)

## Edge Cases and Error Scenarios

### Handwriting Recognition Failures
- Very poor handwriting defaults to image-only storage
- Foreign language text falls back to image search
- User can manually correct recognition mistakes

### Sync Conflicts
- Last-write-wins for individual entries
- Duplicate entries created if major conflicts
- User notified of sync issues with resolution options

### Template Store Issues
- Graceful fallback if store unavailable
- Downloaded templates cached locally
- Clear error messages for purchase failures

## Accessibility Requirements

- VoiceOver support for all interface elements
- Alternative input methods for users who cannot handwrite
- High contrast mode support
- Text size customization
- Voice dictation as handwriting alternative