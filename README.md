Please note all this project has been created without having a clue of code and using prompts on Claude Sonnet 4.5

Skip to line 371 for details on card_designer_v2


================================================================================
DARKWATER ENEMY CARD EDITOR - README
================================================================================

OVERVIEW:
---------
A specialized card design tool for creating enemy cards for the Darkwater 
tabletop game. Features a three-section layout with medieval fonts, behavior 
queues, ability systems, and comprehensive export options.

FILE: enemy_cards.html
VERSION: Enhanced v18
FILE SIZE: ~99 KB


================================================================================
FEATURES
================================================================================

CARD LAYOUT:
-----------
• Three-section design: Left (Artwork), Center (Info), Right (Behavior)
• Medieval-style fonts (Cinzel, Crimson Text)
• Darkwater color scheme (teal #1a4d4d, burgundy #8b1538, cream #f5f3ee)
• Default size: 63.5mm × 88.9mm (poker card dimensions)


SECTION BACKGROUNDS:
-------------------
• Background color picker per section
• Background image upload per section
• Image controls:
  - Scale (50%-150%)
  - Position X/Y (0-100%)
  - Opacity (0-1)
• Clear color/image buttons
• Images use ::before pseudo-elements for layering


CARD CONTENT:
------------
• Enemy Name (large title at top)
• Subtitle (e.g., "Elite Enemy", "Boss")
• Health system with skull node icons
• Behavior Queue (right section) - Add up to 20 behaviors
• Abilities Queue (center section) - Add up to 20 abilities
• Dice progression display (Black/Red/Action dice)
• Weapon icons (20+ icons including swords, axes, bows, shields)


BEHAVIOR QUEUE:
--------------
• Add behaviors with icon, size, and description
• Drag to reorder behaviors
• Delete individual behaviors
• Collapse/expand all behaviors
• Icons scale: 48×48px in behavior loop
• Text formatting for descriptions


ABILITIES QUEUE:
---------------
• Add abilities with icon, name, and description
• Drag to reorder abilities
• Delete individual abilities
• Icon selection from weapon library
• Icons scale: 24×24px in abilities
• Supports multi-line descriptions


HEALTH SYSTEM:
-------------
• Visual health nodes with skull icons
• Adjustable node count (1-20)
• Displays as circular nodes across card
• Skull icons indicate HP


VISUAL CUSTOMIZATION:
--------------------
• Section width adjustment (Left/Center/Right)
• Background colors per section with clear option
• Background images with full positioning controls
• Arrow icon extraction from uploaded images
• Universal image controls (scale, position, opacity)


EXPORT OPTIONS:
--------------
• Export as JPG - High-quality image (2000×2781px)
• Export as PDF - Print-ready PDF format
• Preserves all styling, fonts, and graphics
• Cleans up UI elements before export


STORAGE:
-------
• Saves card data to localStorage
• Auto-saves on changes
• Load saved card data on refresh
• Clear all data option


================================================================================
HOW TO USE
================================================================================

GETTING STARTED:
---------------
1. Open enemy_cards.html in a modern web browser (Chrome, Firefox, Edge)
2. The card editor will load with default settings
3. Start customizing your enemy card


BASIC CARD SETUP:
----------------
1. ENEMY NAME:
   • Click "Enemy Name" field at top
   • Type your enemy's name
   • Text appears in large medieval font

2. SUBTITLE:
   • Click "Subtitle" field
   • Add classification (e.g., "Elite", "Boss", "Minion")

3. HEALTH:
   • Use Health slider or +/- buttons
   • Set number of HP nodes (1-20)
   • Skull icons display across top


SECTION BACKGROUNDS:
-------------------
1. SELECT SECTION:
   • Open "Visual Customization" panel
   • Choose section: Left, Center, or Right

2. ADD COLOR:
   • Click color picker
   • Select background color
   • Click "Clear BG" to remove

3. ADD IMAGE:
   • Click "Choose File" under Background Image
   • Upload image (PNG, JPG, etc.)
   • Adjust controls:
     - Scale: Zoom in/out on image
     - Position X: Move left/right
     - Position Y: Move up/down
     - Opacity: Transparency (0=invisible, 1=solid)
   • Click "Clear BG" to remove image


ADDING BEHAVIORS:
----------------
1. Open "Behavior Queue (Right Section)" panel
2. Click weapon icon dropdown
3. Select icon (sword, axe, bow, etc.)
4. Choose size: Small, Medium, or Large
5. Type behavior description
6. Click "Add Behavior"
7. Behavior appears in right section
8. Drag to reorder (grab and move)
9. Click X to delete


ADDING ABILITIES:
----------------
1. Open "Abilities Queue (Center Section)" panel
2. Click ability icon dropdown
3. Select icon from library
4. Type ability name
5. Type ability description
6. Click "Add Ability"
7. Ability appears in center section
8. Drag to reorder
9. Click X to delete


DICE PROGRESSION:
----------------
• Shows automatically based on card setup
• Displays Black dice, Red dice, and Action icon
• Updates based on behaviors/abilities added


ADJUST SECTION WIDTHS:
---------------------
1. Open "Section Widths" panel
2. Use sliders to adjust:
   • Left Section Width (%)
   • Center Section Width (%)
   • Right Section Width (%)
3. Sections resize in real-time


COLLAPSE/EXPAND:
---------------
• Click "Collapse All" to minimize all behaviors
• Click "Expand All" to show all behaviors
• Useful for reviewing card layout


EXPORTING YOUR CARD:
-------------------
1. Click "💾 Export Card" button at bottom
2. Modal appears with export options:

   EXPORT AS JPG:
   • Click "📸 Export as JPG"
   • High-resolution image downloads
   • Resolution: 2000×2781 pixels
   • Format: JPEG
   • Use for: Digital sharing, printing

   EXPORT AS PDF:
   • Click "📄 Export as PDF"
   • Print-ready PDF downloads
   • Preserves exact dimensions
   • Use for: Professional printing


SAVING YOUR WORK:
----------------
• Card data saves automatically to browser storage
• Data persists between sessions
• Reload page to continue editing
• Clear browser cache to reset


TIPS & TRICKS:
-------------
• Use PNG images with transparency for best results
• Scale images to 100% first, then adjust position
• Higher opacity = more visible background
• Drag behaviors/abilities to reorder anytime
• Collapse all before exporting for clean look
• Test export before final print
• Use clear backgrounds for minimalist designs


TROUBLESHOOTING:
---------------
ISSUE: Card doesn't save
FIX: Check browser localStorage is enabled

ISSUE: Images don't load
FIX: Use supported formats (JPG, PNG, GIF, WebP)

ISSUE: Export looks wrong
FIX: Try different browser (Chrome recommended)

ISSUE: Icons don't show
FIX: Refresh page, clear cache

ISSUE: Background image won't clear
FIX: Click "Clear BG" button, refresh if needed


KEYBOARD SHORTCUTS:
------------------
None currently implemented


BROWSER COMPATIBILITY:
---------------------
✅ Chrome 90+
✅ Firefox 88+
✅ Edge 90+
✅ Safari 14+
❌ Internet Explorer (not supported)


TECHNICAL SPECIFICATIONS:
------------------------
Default Card Size: 63.5mm × 88.9mm (2.5" × 3.5")
Export Resolution: 2000×2781 pixels (300 DPI equivalent)
Color Scheme: Teal (#1a4d4d), Burgundy (#8b1538), Cream (#f5f3ee)
Fonts: Cinzel (headings), Crimson Text (body)
Storage: Browser localStorage
Max Behaviors: 20
Max Abilities: 20
Max Health Nodes: 20


KNOWN LIMITATIONS:
-----------------
• Requires modern browser with localStorage
• Large images may slow performance
• Export requires html2canvas and jsPDF libraries
• No undo/redo functionality
• No multi-card batch editing


CREDITS:
-------
Design Tool: Custom HTML/CSS/JavaScript
Libraries: html2canvas (export), jsPDF (PDF export)
Icon System: Base64-encoded custom icons
Font System: Google Fonts (Cinzel, Crimson Text)


================================================================================
SUPPORT
================================================================================

If you encounter issues:
1. Check browser console for errors (F12)
2. Ensure JavaScript is enabled
3. Try different browser
4. Clear browser cache and reload
5. Check that all external fonts/libraries load


For questions about Darkwater gameplay mechanics or card design best 
practices, consult the Darkwater rulebook.


================================================================================
VERSION HISTORY
================================================================================

v18 (Enhanced):
• Added background color clearing functionality
• Fixed UI interactions
• Improved export quality

v17:
• Section background controls
• Universal image controls
• Arrow extraction feature

v16:
• Multi-ability system
• Ability icon selection
• Drag-and-drop reordering

v15:
• Behavior queue system
• Weapon icon library
• Collapse/expand controls

v14:
• Health node system
• Skull icons
• Visual customization panel

v13:
• Three-panel layout
• Medieval fonts
• Darkwater color scheme

Earlier versions: Initial development


================================================================================
END OF README
================================================================================



Readme universal card designer · TXT
Copy

================================================================================
UNIVERSAL CARD DESIGNER v2.5 - README
================================================================================

OVERVIEW:
---------
A powerful, flexible card design tool for creating custom cards for any game
or purpose. Features include customizable dimensions, grid layouts, drag-and-
drop elements, text formatting, image rotation, section resizing, zoom 
controls, and professional export options.

FILE: card_designer_v2.html
VERSION: 2.5 Enhanced
FILE SIZE: ~64 KB


================================================================================
FEATURES (24 TOTAL)
================================================================================

CARD SYSTEM (3):
---------------
• Adjustable card dimensions (1cm to A2: 42cm × 59.4cm)
• Real-time centimeter measurements (always visible)
• Grid layout system (1-10 rows × 1-10 columns)
• Default: 6.35cm × 8.89cm (poker card size)


SECTION SYSTEM (2):
------------------
• Section background colors (with clear option)
• Section background images with controls:
  - Image opacity (0-100%)
  - Image scale (50-200%)
  - Image position X (0-100%)
  - Image position Y (0-100%)
• **NEW: Drag dividers to resize sections (drag horizontal/vertical lines)**
• Sections tile perfectly (no gaps or overlaps)


ELEMENT SYSTEM (10):
-------------------
• Drag & drop positioning (Photoshop-style)
• 8-point resize handles (corners + edges)
• **NEW: Rotation control (0-360° for images and text)**
• Lock/unlock elements (prevent accidental edits)
• Opacity control (0-100%)
• Constraint mode (free-floating OR constrained to section)
• Duplicate elements (Ctrl+D or button)
• 20 image limit (enforced with counter)
• Layers panel with z-index management
• Image counter display (X/20)


TEXT SYSTEM (5):
---------------
• Full formatting: Bold, Italic, Underline
• Text alignment: Left, Center, Right
• Typography controls:
  - Line height (0.5-3.0)
  - Letter spacing (-5px to 20px)
• 6 web-safe font families (Arial, Helvetica, Times New Roman, Georgia, 
  Courier New, Verdana)
• Font size (8-200px)
• Color picker with 10-color quick palette


WORKFLOW SYSTEM (3):
-------------------
• Undo/Redo (50-state history)
• Save design to JSON file
• Load design from JSON file
• Keyboard shortcuts:
  - Delete: Delete selected element
  - Ctrl+Z: Undo
  - Ctrl+Y: Redo
  - Ctrl+D: Duplicate element


UI ENHANCEMENTS (3):
-------------------
• Snap-to-grid (10px magnetic alignment - toggle on/off)
• 10-color quick palette (Black, White, Red, Green, Blue, Yellow, Magenta,
  Cyan, Orange, Purple)
• Visual feedback (selection outlines, hover effects)


**NEW: ZOOM CONTROL (1):**
-------------------------
• Zoom slider (25%-200%)
• Zoom in (+) and Zoom out (−) buttons
• Fit to screen (⊡) automatic zoom
• Real-time percentage display
• Smooth CSS transform scaling
• Located at bottom center of canvas


EXPORT SYSTEM (3):
-----------------
• Export JPG: High-quality image (2x resolution, 95% quality)
• Export PDF: Standard PDF with exact dimensions (3x resolution)
• Export Print-Ready PDF:
  - 4x resolution for professional printing
  - 3mm bleed on all sides
  - Crop marks at corners
  - PDF metadata included


================================================================================
HOW TO USE
================================================================================

GETTING STARTED:
---------------
1. Open card_designer_v2.html in a modern web browser
2. The designer loads with a default poker-sized card (6.35cm × 8.89cm)
3. Use left sidebar for properties, right sidebar for layers
4. Canvas in center with zoom controls at bottom


SETTING UP YOUR CARD:
--------------------

1. CARD DIMENSIONS:
   • Find "Card Dimensions (cm)" in left sidebar
   • Enter width (1-42cm, max A2 width)
   • Enter height (1-59.4cm, max A2 height)
   • Measurements update in real-time above canvas

2. GRID LAYOUT:
   • Find "Grid Layout" section
   • Set Rows (Y): 1-10
   • Set Columns (X): 1-10
   • Click "Update Grid" button
   • Sections appear as tiled grid on card

3. SNAP TO GRID (OPTIONAL):
   • Check "Snap to Grid (10px)" checkbox
   • Elements will magnetically align to 10px grid
   • Useful for precise alignment


WORKING WITH SECTIONS:
---------------------

SELECTING A SECTION:
• Click anywhere on a section
• Section highlights with teal outline
• Properties panel shows section controls

SECTION BACKGROUND COLOR:
1. Select a section
2. Click color picker
3. Choose color
4. OR click a color from quick palette
5. Click "Clear Color" to remove

SECTION BACKGROUND IMAGE:
1. Select a section
2. Click "Choose File" under Background Image
3. Upload image (PNG, JPG, GIF, WebP)
4. Image controls appear:
   • Opacity slider (0-1): Transparency
   • Scale slider (50-200%): Zoom
   • Position X (0-100%): Horizontal placement
   • Position Y (0-100%): Vertical placement
5. Click "Clear Image" to remove

**NEW: RESIZING SECTIONS:**
1. Hover over line between sections
2. Teal resize handle appears (8px wide)
3. Click and drag:
   • Horizontal lines: Resize row heights
   • Vertical lines: Resize column widths
4. One section grows, adjacent section shrinks
5. Release to finalize
6. Minimum section size: 50px


ADDING ELEMENTS:
---------------

ADDING IMAGES:
1. Click "🖼 Add Image" button in toolbar
2. Note: Maximum 20 images (counter shows X/20)
3. Select image file
4. Image appears on canvas (center position)
5. Drag to reposition
6. Use handles to resize
7. Adjust properties in left sidebar

ADDING TEXT:
1. Click "T Add Text" button in toolbar
2. Text box appears with "Double-click to edit"
3. Click on text in properties panel
4. Edit content, formatting, alignment
5. Drag to reposition
6. Use handles to resize


WORKING WITH ELEMENTS:
---------------------

SELECTING ELEMENTS:
• Click element on canvas
• OR click element in Layers panel (right sidebar)
• Selected element shows dashed teal outline
• Transform handles appear around element

MOVING ELEMENTS:
• Click and drag element
• Element follows cursor
• Stays within canvas boundaries
• Constraint mode affects movement (see below)

RESIZING ELEMENTS:
• Select element
• Grab any of 8 handles:
  - Corners (NW, NE, SE, SW): Diagonal resize
  - Edges (N, E, S, W): Single-axis resize
• Drag to resize
• Minimum size: 20×20px

**NEW: ROTATING ELEMENTS:**
1. Select an image or text element
2. Find "Rotation (degrees)" slider in properties
3. Drag slider (0-360°) or type value
4. Element rotates in real-time
5. Rotation angle shows in layers panel
6. Works with drag, resize, and all other features

ELEMENT OPACITY:
• Select element
• Drag "Opacity" slider (0-1)
• 0 = invisible, 1 = fully opaque
• Useful for watermarks or subtle effects

LOCKING ELEMENTS:
• Select element
• Click "🔓 Lock Element" button
• Locked elements cannot be moved or resized
• Icon changes to 🔒
• Click again to unlock

DELETING ELEMENTS:
• Select element
• Click "🗑 Delete" button
• OR press Delete key
• Element removed from canvas and layers


TEXT FORMATTING:
---------------

BASIC TEXT EDITING:
1. Select text element
2. "Text Properties" panel appears
3. Type in "Text Content" field
4. Changes appear in real-time

FONT SETTINGS:
• Font Family: Choose from 6 web-safe fonts
• Font Size: 8-200px (type or use arrows)
• Text Color: Click color picker OR quick palette

TEXT FORMATTING:
• Click "B" button: Toggle bold
• Click "I" button: Toggle italic
• Click "U" button: Toggle underline

TEXT ALIGNMENT:
• Click "◀" button: Align left
• Click "■" button: Align center
• Click "▶" button: Align right

ADVANCED TYPOGRAPHY:
• Line Height: 0.5-3.0 (space between lines)
• Letter Spacing: -5 to 20px (space between letters)


CONSTRAINT MODE:
---------------
Each element has a constraint mode:

FREE-FLOATING (default):
• Element can be placed anywhere on card
• Moves freely across all sections
• Not bound to any section

CONSTRAINED TO SECTION:
1. Select element
2. Change "Constraint Mode" to "Constrained to Section"
3. Element can only move within its current section
4. Useful for keeping elements organized


LAYERS MANAGEMENT:
-----------------
Right sidebar shows all elements as layers:

VIEWING LAYERS:
• Image counter at top (X/20 images)
• Each element shown as card with:
  - Icon (🖼 for images, T for text)
  - Name (Image #1, Text #2, etc.)
  - Rotation angle if rotated (45°)
  - Type label

SELECTING FROM LAYERS:
• Click any layer card
• Element selects on canvas
• Properties panel updates

REORDERING LAYERS (Z-INDEX):
• Click ↑ button: Move layer up (closer to front)
• Click ↓ button: Move layer down (closer to back)
• Top layer in list = front of card
• Bottom layer in list = back of card

LOCKING FROM LAYERS:
• Click 🔓/🔒 button on layer
• Toggles lock state


DUPLICATING ELEMENTS:
--------------------
1. Select element
2. Click "📋 Duplicate Element" button
3. OR press Ctrl+D
4. Copy appears offset by 20px
5. Immediately selected for editing


**NEW: ZOOM CONTROLS:**
-----------------------
Located at bottom center of canvas:

ZOOM CONTROLS OVERVIEW:
• [−] Zoom Out button
• [⊡] Fit to Screen button
• [━━━━○━━━━] Zoom slider (25%-200%)
• [100%] Percentage display
• [+] Zoom In button

ZOOMING IN:
• Click [+] button (increases by 10%)
• OR drag slider to right
• Maximum zoom: 200%

ZOOMING OUT:
• Click [−] button (decreases by 10%)
• OR drag slider to left
• Minimum zoom: 25%

FIT TO SCREEN:
• Click [⊡] button
• Automatically calculates optimal zoom
• Entire card fits in visible area
• Useful after changing card dimensions

MANUAL ZOOM:
• Drag slider to any position
• Adjusts in 5% increments
• Percentage updates in real-time
• Card scales smoothly from center

ZOOM NOTES:
• Zoom only affects view, not actual card size
• Export uses actual dimensions (not zoomed)
• Zoom resets to 100% on page reload
• Smooth CSS transform (no quality loss)


UNDO/REDO:
---------
• Click "↶ Undo" button (or Ctrl+Z)
• Click "↷ Redo" button (or Ctrl+Y)
• 50 states saved in history
• Tracks: element changes, moves, resizes, rotations, section changes, etc.


SAVING YOUR DESIGN:
------------------
1. Click "💾 Save Design" button
2. JSON file downloads: card-design-[timestamp].json
3. File contains:
   - Card dimensions and grid settings
   - All sections with backgrounds
   - All elements with properties
   - Section custom sizes
   - Rotation values

LOADING A DESIGN:
1. Click "📁 Load Design" button
2. Select saved JSON file
3. Card restores exactly as saved
4. All elements, positions, rotations load


EXPORTING YOUR CARD:
-------------------

EXPORT AS JPG:
1. Click "📸 Export JPG" button
2. High-quality JPEG downloads
3. Resolution: 2× actual size
4. Quality: 95%
5. File: card-design-[timestamp].jpg
6. Use for: Digital sharing, web, preview

EXPORT AS PDF:
1. Click "📄 Export PDF" button
2. Standard PDF downloads
3. Resolution: 3× actual size
4. Exact dimensions in millimeters
5. File: card-design-[timestamp].pdf
6. Use for: General printing, digital distribution

EXPORT AS PRINT-READY PDF:
1. Click "🖨 Print-Ready PDF" button
2. Professional print PDF downloads
3. Resolution: 4× actual size
4. 3mm bleed on all sides
5. Crop marks at corners
6. PDF metadata included
7. File: card-design-print-ready-[timestamp].pdf
8. Use for: Professional printing, print shops

EXPORT NOTES:
• All UI elements hidden during export
• Selection outlines removed
• Measurements, rulers, handles hidden
• Rotation preserved in exports
• Actual card size used (not zoom level)


KEYBOARD SHORTCUTS:
------------------
Delete        Delete selected element
Ctrl+Z        Undo last action
Ctrl+Y        Redo last action
Ctrl+D        Duplicate selected element


================================================================================
TIPS & TRICKS
================================================================================

GENERAL TIPS:
• Start by setting card dimensions first
• Use grid layout to organize sections
• Snap-to-grid helps with precise alignment
• Lock elements when finalized to prevent accidents
• Use layers panel for easy selection
• Save your work frequently (no auto-save)

IMAGE TIPS:
• Use PNG images for transparency support
• Upload high-resolution images for better quality
• Images maintain aspect ratio when resizing from corners
• Rotate images for creative layouts
• Use opacity for watermark effects

TEXT TIPS:
• Start with larger font size, reduce as needed
• Use line height for better readability
• Letter spacing useful for titles/headers
• Alignment affects entire text box
• Duplicate text boxes to maintain consistent formatting

SECTION TIPS:
• Resize sections by dragging dividers for custom layouts
• Use section backgrounds for zones (header, footer, content)
• Background images can create themes
• Adjust image position for focal points
• Lower opacity for subtle backgrounds

ZOOM TIPS:
• Use Fit to Screen after changing card size
• Zoom in (150-200%) for detail work
• Zoom out (25-50%) to see overall design
• Zoom doesn't affect export quality

WORKFLOW TIPS:
• Design workflow: Layout → Backgrounds → Elements → Text → Export
• Use constraint mode to keep elements in sections
• Test exports before final print
• Save multiple versions for variations


================================================================================
TROUBLESHOOTING
================================================================================

ISSUE: Can't add more images
FIX: 20 image limit reached. Delete unused images.

ISSUE: Element won't move
FIX: Check if element is locked (🔒). Unlock to edit.

ISSUE: Section won't resize
FIX: Can only resize between adjacent sections. Check grid layout.

ISSUE: Rotation not working
FIX: Select element first, then adjust rotation slider.

ISSUE: Zoom controls not visible
FIX: Check bottom center of canvas. May be hidden if browser window small.

ISSUE: Export quality poor
FIX: Use larger card dimensions. Export scales from actual size.

ISSUE: Undo/Redo disabled
FIX: At beginning/end of history. Make changes to enable.

ISSUE: Loaded design looks wrong
FIX: Ensure file is valid JSON from this tool. Check browser console.

ISSUE: Snap-to-grid too aggressive
FIX: Uncheck "Snap to Grid" checkbox for free movement.

ISSUE: Can't select element
FIX: Check if behind another element. Use layers panel instead.


================================================================================
BROWSER COMPATIBILITY
================================================================================

FULLY SUPPORTED:
✅ Chrome 90+
✅ Firefox 88+
✅ Safari 14+
✅ Edge 90+

NOT SUPPORTED:
❌ Internet Explorer (any version)
❌ Browsers without ES6 support
❌ Browsers without Canvas API


REQUIRED FEATURES:
• JavaScript enabled
• Canvas API support
• FileReader API (for image uploads)
• CSS transforms
• localStorage (for future features)


================================================================================
TECHNICAL SPECIFICATIONS
================================================================================

FILE SIZE: 64.4 KB (HTML + CSS + JavaScript)
LINES OF CODE: 2,162
JAVASCRIPT LINES: 1,397
EVENT LISTENERS: 48
FEATURES: 24 major features
STATE HISTORY: 50 undo/redo states

CARD DIMENSIONS:
• Minimum: 1cm × 1cm
• Maximum: 42cm × 59.4cm (A2 paper size)
• Default: 6.35cm × 8.89cm (poker card)
• Input precision: 0.1cm

GRID SYSTEM:
• Min rows/cols: 1
• Max rows/cols: 10
• Total sections: 1-100
• Section min size: 50px

ELEMENT LIMITS:
• Max images: 20 (enforced)
• Max text elements: Unlimited
• Min element size: 20×20px
• Rotation range: 0-360°
• Opacity range: 0-1 (0-100%)

ZOOM:
• Range: 25%-200%
• Step: 5% (slider)
• Button increment: 10%
• Default: 100%
• Transform: CSS scale()

EXPORT:
• JPG: 2× resolution, 95% quality, RGB
• PDF: 3× resolution, exact mm dimensions
• Print PDF: 4× resolution, 3mm bleed, crop marks

TEXT:
• Font size: 8-200px
• Line height: 0.5-3.0
• Letter spacing: -5px to 20px
• Font families: 6 web-safe
• Alignment: 3 options
• Formatting: Bold, Italic, Underline

COLORS:
• Quick palette: 10 colors
• Custom color picker: 16.7M colors
• Opacity: 0-100% for all elements


================================================================================
DEPENDENCIES
================================================================================

EXTERNAL LIBRARIES (CDN):
• html2canvas v1.4.1 - For canvas capture during export
• jsPDF v2.5.1 - For PDF generation

Both libraries load from CDN (Content Delivery Network).
Internet connection required for export features.


================================================================================
VERSION HISTORY
================================================================================

v2.5 (Current):
• Added zoom/magnifying lens control (25-200%)
• Zoom slider with +/- buttons and fit-to-screen
• Fixed syntax errors
• Enhanced stability

v2.4:
• Added image rotation control (0-360°)
• Added section grid resizing (drag dividers)
• Rotation indicator in layers
• Section dimension persistence

v2.3 (MVP):
• Added text formatting (B/I/U)
• Added text alignment (L/C/R)
• Added line height & letter spacing controls
• Added 20 image limit enforcement
• Added constraint mode (free/section)
• Added snap-to-grid (10px)
• Added color palette (10 colors)
• Added keyboard shortcuts
• Added duplicate element feature

v2.2:
• Added drag & drop with transform handles
• Added 8-point resize handles
• Added working undo/redo (50 states)
• Added load design functionality

v2.1:
• Added section background controls
• Added section image positioning

v2.0:
• Initial universal designer
• Card dimensions system
• Grid layout system
• Basic element system


================================================================================
KNOWN LIMITATIONS
================================================================================

• No auto-save (must manually save)
• No collaborative editing
• No custom font upload (web-safe fonts only)
• No vector graphics support (raster images only)
• No text shadow/stroke effects
• No gradient fills
• No image filters/effects
• No shape tools (rectangles, circles, etc.)
• No grouping of elements
• No alignment guides (only snap-to-grid)
• Export requires internet (for CDN libraries)
• Zoom state not saved (resets to 100%)


================================================================================
FUTURE ENHANCEMENTS (POTENTIAL)
================================================================================

• Auto-save functionality
• Custom font upload
• Shape tools (rectangle, circle, polygon)
• Image filters (grayscale, sepia, blur)
• Text effects (shadow, stroke, gradient)
• Gradient backgrounds
• Alignment guides and smart guides
• Element grouping
• Multi-card projects
• Templates system
• Batch export
• Color themes
• Rulers with measurements


================================================================================
CREDITS
================================================================================

Design Tool: Custom HTML/CSS/JavaScript
Export Libraries: html2canvas (MIT), jsPDF (MIT)
Architecture: Single-page application (SPA)
State Management: Custom implementation
Rendering: Canvas API + DOM manipulation


================================================================================
SUPPORT
================================================================================

For issues:
1. Check browser console (F12) for errors
2. Verify browser compatibility
3. Ensure JavaScript is enabled
4. Clear cache and reload
5. Try different browser
6. Check internet connection (for export)

Common error codes:
• "Maximum of 20 images reached" - Delete unused images
• "Error loading design" - JSON file corrupted or invalid
• "Export failed" - Check internet connection for CDN libraries


================================================================================
LICENSE
================================================================================

This tool is provided as-is for personal and commercial use.
External libraries (html2canvas, jsPDF) have their own licenses (MIT).


================================================================================
END OF README
================================================================================
