# AI CODING HANDOFF: Developer Tool Workspace

> Comprehensive Product → UX → Design Intent → Technical Implementation Blueprint
> Generated on: 2026-09-14 | Schema: V2 | Target: OpenCode, Codex, Cline, Cursor, Antigravity

---

## 1. PRODUCT DEFINITION
- **Project Name**: Planner V2
- **Description**: Visual AI project planning system bridging PRD, UX decisions, Design Intent, and AI Coding Handoff.
- **Project Scope**: Greenfield Build

---

## 2. UX DEFINITION & STATE FEELINGS
- **First Visit / Onboarding**: Clear visual hierarchy, uncluttered introduction, immediate access to value.
- **Empty State**: Quiet, instructional, actionable with sample template trigger.
- **Input & Editing State**: Real-time inline feedback, visible keyboard focus indicators.
- **Loading State**: Context-aware skeleton loaders without layout shift.
- **Success State**: Instant inline confirmation without disruptive modal popups.
- **Error State**: Explicit root-cause message with inline recovery actions.
- **Mobile Viewport**: Preserved single-column visual hierarchy, minimum touch targets 44x44px.

---

## 3. DESIGN INTENT BRIEF

### 1. DESIGN NORTH STAR
> **"Technical, calm, information-dense, and precise — like a professional engineering workspace rather than a generic SaaS dashboard."**

### 2. VISUAL DIRECTION
- **Direction**: Editorial Utility
- **Rationale**: High information density with clear typography and structured sections for fast visual scanning.

### 3. VISUAL METAPHOR
- **Real-World Reference**: Developer terminal + technical documentation workbook
- **Impact on Layout & Components**: Drives crisp grid lines, deliberate contrast, and functional typography over decorative cards.

### 4. VISUAL REFERENCES & PRINCIPLES
- **Reference**: Developer Terminal & Workbench
- **What to Borrow**: Data density, tabular monospace typography, high contrast border hierarchy.
- **What NOT to Copy**: Exact proprietary layout, branding elements, monochrome dullness.

### 5. LAYOUT STRATEGY
- **Container & Grid**: Max-width 1280px with narrow centered utility shells | 2-column split view
- **Primary Focal Point**: Primary calculated result / central planning canvas
- **Desktop**: Two-column split view (Input/Canvas on left + Result/Context on right)
- **Mobile**: Linear stacked step-by-step navigation
- **Whitespace Philosophy**: Intentional around primary content, minimal between related utility controls

### 6. TYPOGRAPHY DIRECTION
- **Display**: Clean geometric sans with strict weight hierarchy
- **Body**: Neutral system sans (Inter / system sans)
- **Numeric & Data**: Tabular monospace for statistics, metrics, and identifiers
- **Communication Style**: Dense and utilitarian
- **Monospace Rule**: Use monospace selectively for data schemas, code snippets, and structural IDs.

### 7. COLOR DIRECTION
- **Primary Role**: Deep slate background with crisp light gray typography
- **Accent Role**: Teal/Cyan highlight for active elements and key metrics
- **Surface Character**: Subtle dark borders with dark slate surfaces
- **Contrast Expectations**: High contrast (WCAG AAA compliant text) for optimal readability

### 8. COMPONENT CHARACTER
- **General Styling**: Restrained and functional
- **Borders & Radius**: Subtle 1px slate-800 borders | Radius: Small to medium (rounded-lg 8px), never pill-soup
- **Shadows**: Minimal subtle elevation only for floating overlays
- **Cards**: Use sparingly; avoid card soup.
- **Buttons**: Primary action visually dominates secondary utility buttons.
- **Inputs**: Feel like utility controls with explicit state feedback.
- **Icons**: Functional only for scanning; no decorative icon spam.

### 9. INTERACTION CHARACTER
- **Philosophy**: Immediate feedback, direct manipulation, keyboard-friendly
- **Motion Intensity**: Subtle & instantaneous (<150ms), zero decorative bounce
- **Motion & States**: Subtle instantaneous state transitions without excessive delays

### 10. DENSITY
- **Overall Level**: BALANCED
- **Specific Rules**: Results and technical data dense; primary controls and onboarding spacious.

### 11. RESPONSIVE BEHAVIOR
- **Breakpoint Behavior**: Desktop side-by-side collapses into logical stacked workflow on mobile.
- **Mobile Priority**: Primary output and core input action remain visible without horizontal scroll.

### 12. ACCESSIBILITY INTENT
- Visible focus outlines on keyboard navigation
- WCAG AA contrast ratios
- Semantic HTML layout elements
- Screen reader accessible labels
- Reduced motion query support

### 13. ANTI-PATTERNS (MUST NOT APPEAR)
- generic SaaS dashboard clichés
- excessive rounded cards / card soup
- gradient-heavy UI without semantic meaning
- glassmorphism or heavy blur effects
- decorative icons lacking purpose
- meaningless pill badges on every label
- fake AI sparkles and floating animations
> **Overcorrection Warning**: Avoiding gradients or cards does not mean making the UI flat or monochrome.

### 14. VISUAL ACCEPTANCE CRITERIA
- [ ] The primary output/result is immediately recognizable and visually dominant at a 2-second glance.
- [ ] The design does not resemble a generic AI-generated SaaS template.
- [ ] Keyboard navigation allows full operation without mouse interaction.
- [ ] Desktop and mobile viewports maintain visual hierarchy without stacked chaos.

---

## 4. IMPLEMENTATION RULES FOR CODING AGENTS
1. **Inspect Before Modifying**: Always read existing files, types, and components before writing code.
2. **Preserve Working Architecture**: Do not rewrite existing working components or change build systems unless instructed.
3. **Follow Design Intent**: Ground every visual choice in the Design North Star, Visual Metaphor, and Typography/Color direction.
4. **Enforce Intentional Composition**: Spacing, sizing, and borders must have semantic purpose, not random copy-paste.
5. **Strict Anti-AI-Slop Rules**: Zero generic gradient blobs, zero card soup, zero glassmorphism, zero decorative icon spam.
6. **Atomic Verification**: Build and test after every significant change.
7. **Execute Visual Verification**: Follow the mandatory 15-step verification loop below before claiming completion.

---

## 5. VISUAL VERIFICATION LOOP (15-STEP SEQUENCE)
1. Inspect existing project.
2. Understand current implementation.
3. Plan changes.
4. Implement.
5. Run the application.
6. Render desktop viewport (~1280px-1440px).
7. Render mobile viewport (~390px).
8. Inspect screenshots / browser output.
9. Identify highest-impact visual problem.
10. Fix that problem.
11. Render again.
12. Repeat if necessary.
13. Run functional tests.
14. Run typecheck / build / lint.
15. Final visual inspection.

---

## 6. DESIGN CRITIQUE STAGE (PRIORITY HIERARCHY)
- **P0 — Broken (Fix First!)**: Layout breakage, text overflow, inaccessible touch targets, runtime crash.
- **P1 — Visual Hierarchy (Fix Second!)**: Focal point clarity, purposeful spacing density, typography contrast.
- **P2 — Micro Polish (Fix Last!)**: Subtle 1px border alignment, smooth hover feedback, quiet empty states.

---

## 7. DESIGN JUDGMENT GATE (10 QUESTIONS)
1. Does the rendered UI express the Design North Star?
2. Is the primary focal point obvious at a 2-second glance?
3. Does the visual metaphor actually influence layout and typography?
4. Does the composition feel intentional rather than assembled from generic template kits?
5. Is whitespace purposeful rather than uniform filler?
6. Are components visually differentiated according to their semantic roles?
7. Does the interface feel like a coherent product rather than floating cards?
8. Is the design recognizable without relying solely on a logo?
9. Does it strictly avoid all specified anti-patterns?
10. Would a human designer consider another iteration materially worthwhile? (If YES: iterate!)
