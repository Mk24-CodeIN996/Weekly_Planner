# Weekly Planner - Design Philosophy

## Chosen Approach: **Minimalist Productivity**

### Design Movement
Inspired by Bauhaus principles and modern productivity apps (Notion, Linear). Clean, purposeful, with subtle depth and micro-interactions that reward focus and intentionality.

### Core Principles
1. **Clarity First**: Every element serves a purpose. Information hierarchy is crystal clear.
2. **Subtle Depth**: Soft shadows, gentle transitions, and minimal gradients create dimension without distraction.
3. **Intentional Whitespace**: Breathing room between sections emphasizes content and reduces cognitive load.
4. **Micro-interactions**: Smooth transitions and responsive feedback make the interface feel alive and responsive.

### Color Philosophy
- **Light Mode**: Soft off-white background (`#FAFAFA`), warm neutral grays for text, subtle blue accents for CTAs and active states
- **Dark Mode**: Deep charcoal background (`#1A1A1A`), light gray text, the same blue accents for consistency
- **Accent Color**: Warm blue (`#3B82F6`) for interactive elements, progress indicators, and focus states
- **Reasoning**: The palette is calming and professional, reducing eye strain during extended use while maintaining clear visual hierarchy

### Layout Paradigm
- **Asymmetric Grid**: Profile section floats in the top-left corner; countdown circle anchors the top-right; main content flows naturally below
- **Breathing Sections**: Clear visual separation between header, countdown, weekly table, and navigation
- **Responsive Stacking**: On mobile, elements stack vertically while maintaining visual hierarchy

### Signature Elements
1. **Countdown Circle**: A large, animated circular progress indicator showing days remaining—becomes the focal point of the interface
2. **Subtle Border Accents**: Thin, soft borders (`1px` in muted color) separate sections without harsh divides
3. **Smooth Transitions**: All interactive elements (buttons, inputs, theme toggle) transition smoothly over 200-300ms

### Interaction Philosophy
- **Immediate Feedback**: Buttons scale slightly on click; inputs highlight with a soft glow on focus
- **Hover States**: Subtle color shifts and shadow increases on hover
- **Theme Toggle**: Smooth fade transition between light and dark modes
- **Data Editing**: Inline editing with smooth focus states and clear save indicators

### Animation
- **Entrance**: Elements fade in with a slight upward motion (100-200ms ease-out)
- **Hover**: Buttons scale to 98% with a soft shadow increase (150ms ease-out)
- **Focus**: Input fields glow with a subtle blue shadow (200ms ease-out)
- **Theme Switch**: Background and text fade smoothly (300ms ease-in-out)
- **Countdown Update**: The circle pulses gently when the countdown changes
- **Respect Motion**: All animations respect `prefers-reduced-motion`

### Typography System
- **Display Font**: `Poppins` (600-700 weight) for headings and the countdown number—modern, friendly, clear
- **Body Font**: `Inter` (400-500 weight) for body text and inputs—highly readable, neutral
- **Hierarchy**: 
  - Countdown number: `Poppins 700` at `3rem`
  - Section headings: `Poppins 600` at `1.5rem`
  - Table headers: `Poppins 600` at `1rem`
  - Body text: `Inter 400` at `0.95rem`

### Brand Essence
**Positioning**: A calm, focused weekly planning tool that respects your time and attention.  
**Personality**: Thoughtful, reliable, minimalist, empowering.

### Brand Voice
- Headlines: Direct, action-oriented ("Plan Your Week", "Set Your Target")
- CTAs: Clear and concise ("Save", "Update", "Set Date")
- Microcopy: Helpful and encouraging ("No weeks yet—start planning!", "Days remaining")
- Avoid: Generic filler like "Welcome" or "Get started today"

### Wordmark & Logo
A simple, bold geometric mark: a circle with a checkmark inside, symbolizing completion and focus. No text—just the mark in the accent blue color.

### Signature Brand Color
**Warm Blue** (`#3B82F6`): Calm, trustworthy, and energizing—perfect for a productivity tool.

---

## Implementation Notes
- Use Tailwind's built-in spacing and color utilities to maintain consistency
- Leverage shadcn/ui components for form inputs and dialogs
- Implement localStorage for all data persistence
- Ensure dark/light mode toggle is always accessible in the header
- Test animations on reduced-motion devices
