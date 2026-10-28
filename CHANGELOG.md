# SwitchRig App Changelog

All notable changes, manufacturing updates, and component catalog additions to SwitchRig App are documented in this file.

---

## [v0.9.0] (October 28, 2026)

### Added
* Privacy Policy Page: New dedicated `/privacy` route with consent plumbing and sitemap refresh.
* X-Ray Shell View: New floating-dock toggle that ghosts enclosure walls and rear panel in 3D views (off by default).
* LED Halo Color Picker: Stainless hardware now offers a ring-LED color picker (red, green, blue, amber, white).
* LED Telemetry Animations: WS2812B matrices play a rotating demo sequence â€” proximity side bars, yellow flag, red flag, and RPM sweep.
* Recommended-Path Pulse: The welcome modal's demo button glows to guide first-time users.

### Improved
* Explode Slider Dock: The explosion control lives in the floating viewport dock with a layout-stable design across assembled and exploded views.
* Demo GT3 Box Refresh: Added twist-release E-stop, ABS button pair, QR codes on both side frames, and a deeper 64mm enclosure.
* Stainless Vandal Buttons: Rebuilt as brushed stainless steel with flat actuators and recessed illuminated halo rings; body colors and finishes no longer apply to metal hardware.
* E-Stop Model: Added the missing plunger stalk connecting the mushroom dome to the collar.

### Fixed
* Explode Slider Bounce-Back: Resolved an issue where dragging the slider to 0% (or any value below 20%) snapped back to 45% on hold or release.
* Mobile Dock Overflow: Resolved floating-dock collisions on compact viewports caused by the wider toggle row.

---

## [v0.8.3] (October 27, 2026)

### Improved
* Responsive Mobile Menu Bar: Redesigned the top navigation into a clean two-tier layout on compact screens, displaying brand identity, quick actions, and all five workspace modes simultaneously without overlapping controls.
* Mobile Sidebar Access: Added dedicated Setup and Inspect buttons directly to the mobile navigation bar, providing instantaneous one-tap access to component configuration and design rule diagnostics.
* Default Viewport Framing: Optimized initial 3D camera distance and 2D canvas scale on mobile devices, ensuring complete enclosure assemblies and mounting flanges remain fully visible with generous margins upon loading.
* Touchscreen Status Bar: Streamlined bottom status readouts and explosion spread controls on mobile screens, preserving tactile switch actuation feedback without crowding cookie preference or audio toggles.

### Fixed
* Viewport Control Collision: Resolved an issue where the template selector overlapped floating camera angle presets on mobile screens.
* Floating Bar Clipping: Corrected an off-screen overflow defect where the 3D view preset bar extended beyond the left viewport boundary on compact viewports.
* Modal Action Button Fit: Corrected welcome modal card constraints so action buttons fit cleanly inside card borders without protruding below margins.
* Nested Cut Sheet Collapse: Resolved a flexbox shrinking issue in the nesting view that caused the laser machine bed to compress on mobile displays.
* Mirrored Wiring Framing: Corrected vertical positioning in the wiring companion view to prevent top-level diagram clipping on mobile phones.

---

## [v0.8.2] (October 27, 2026)

### Improved
* Landing Modal Layout: Optimized card proportions across mobile and desktop displays so both the GT3 demo and blank enclosure options present clean, equal-height layouts with full text and action button visibility.
* Mobile Modal Scrolling: Ensured reliable vertical scrolling on mobile phones across all configuration dialogs without clipping or overlapping content.
* Privacy Banner Layering: Refined z-index stacking so the consent notice remains accessible without obstructing active design dialogs.

### Fixed
* Card Collapse Defect: Resolved an issue where the recommended GT3 demo card collapsed to a narrow strip on mobile devices.
* Modal Flex Shrinkage: Corrected flexbox scroll behavior to prevent modal bodies from resisting scroll activation on compact touchscreens.

---

## [v0.8.1] (October 27, 2026)

### Added
* Mobile Viewport-First Off-Canvas Drawers: Complete mobile responsiveness giving phones and tablets a full-bleed 100% width 3D and 2D canvas by default.
* Floating Mobile Action Pills: Thumb-accessible floating action pills (Configure and Inspect) on mobile for on-demand access to design steps and component inspection with active DRC warning badges.
* Single-Drawer Mutual Exclusivity: Strictly permits only one sidebar open at a time on mobile to maximize viewport visibility and eliminate UI overlap.

### Fixed
* Mobile Modal Clipping: Resolved height overflow in Welcome, Matrix, and Custom Laser modals with dynamic mobile viewport height (100dvh) and independent scrolling containers.
* Mobile Viewport Compression: Fixed layout defect where fixed 320px left and right docks previously crushed the center viewport to 0px on mobile screens.
* Mobile Touch Targets: Upgraded all primary buttons across mobile modals to meet the 48px touch target standard.
* Horizontal Canvas Overflow: Converted sidebar widths to fluid relative units preventing side-scroll overflow on narrow screens.

---

## [v0.8.0] (October 26, 2026)

### Added
* 3D Internal Wire Harness Simulation: Procedural silicone wire harness connecting hardware terminals to an onboard microcontroller with red ground and multi-color signal routing, enabled by default in 3D views.
* Multi-Surface Markings & Custom Branding: Support for custom laser etch and CNC V-carve markings across all 6 enclosure faces (front, top, bottom, left, right, rear) resting flush on panel faces.
* Custom Border Framing Modes: Laser and CNC machinable vector border styles (Underline, Outline Rectangle, and Pill Contour) with zero solid area fills.
* Procedural QR Code Generator: Vector QR matrix generator allowing users to embed live telemetry links, pinouts, or documentation URLs directly onto fabrication sheets and 3D models.
* Typography Engine: Integrated Google Web Fonts library supporting modern sans, cockpit monospace, industrial stencil, and racing display typefaces.
* Markings Design Rule Check (DRC): Real-time collision detection verifying clearance between custom text/QR markings and component cutouts with 1-click automatic repositioning.

### Improved
* High-Performance 60fps GPU Explode Easing: Completely decoupled axial explosion kinematics and range slider scrubbing from 3D CAD mesh geometry rebuilds, delivering locked 60fps motion without frame drops.
* Missile Safety Canopy Kinematics: Canopy open/closed settings persist seamlessly across viewport transitions, animating closed in assembled view and open in exploded view.
* 2D & 3D Markings Alignment: Synchronized text/QR positioning, scale, and rotations between 2D vector CAD workplanes and 3D Three.js decals.

### Fixed
* Net-New Exploded View State: Corrected issue where new sessions in exploded view mode defaulted to 0% assembled view rather than the default 45% explosion span.
* Text Overlap in Demo Template: Resolved collision where adjacent switches shared overlapping default label spaces.

---

## [v0.7.0] (October 26, 2026)

### Added
* Blueprint Dimension Overlay: Added an interactive toggle across 2D CAD and 3D Studio views rendering high contrast dimensional callout badges.
* SketchUp Style Dimension Bookends: Procedural dimension lines with bookend ticks detailing Width, Height, and Thickness for individual faceplates, walls, and rear panels.
* Enhanced Readout Legibility: Dimension callout badges and witness text default to larger bold typography for immediate legibility at standard zoom levels.
* v0.1.0 Changelog Archive: Backfilled immutable history documentation for v0.1.0 in the public community repository.

### Improved
* Cockpit Monospace Header Branding: Restyled brand wordmark with clean Cockpit Monospace typography presenting SWITCH RIG in pure white with de-emphasized domain styling.
* 2D CAD Workspace Spacing: Re-spaced top viewport toolbar to eliminate collision between the New Template launcher and the floating scale indicator.
* Dynamic Silkscreen Label Placement: Programmatic positioning engine prevents component labels such as RPM and Shift lights from overlapping adjacent hardware on any custom box layout.
* Nested Cut Sheet Packing: Resolved part collision between spare fastener rings and the rear panel in the master cut sheet nesting view.

### Fixed
* Cut Sheet Vector Etch Lines: Eliminated superfluous horizontal blue etch guide lines on the front faceplate and master vector cut sheets.
* Cut Sheet Faceplate Orientation: Corrected inverted vertical orientation of the front faceplate on fabrication cut sheets.
* Dimension Line Corner Junctions: Simplified 2D Width and Height dimension lines to a clean 90-degree intersection with zero slash ticks or ornamental gaps.

---

## [v0.6.0] (October 25, 2026)

### Added
* Community Documentation Showcase: Integrated high-resolution studio viewports into public documentation displaying photorealistic 3D assembly, parametric 2D vector CAD layouts, and exploded mechanical interlock views.
* Viewport Docked Status Bar: Integrated persistent status bar across 2D CAD and 3D Studio viewports consolidating live tactile actuation indicators, procedural audio mute toggle, exploded view slider controls, and cookie preferences trigger.
* Public Community Issue Suite: Launched official community repository featuring structured issue templates for arcade switch footprints, laser and CNC machine profiles, CAD layout feature requests, and bug reports.
* Decoupled Cookie Preferences Modal: Users can inspect, customize, or revoke consent preferences on demand directly from the studio status bar.

### Improved
* Studio Header Layout: Streamlined top navigation bar with simplified branding and relocated project template triggers into the viewport canvas.
* Onboarding Flow: Decoupled the welcome dialog from internal application release versions.
* Responsive Mobile & Tablet Layout: Optimized viewport status bar and canvas controls across narrow and wide aspect ratios.

---

## [v0.5.0] (October 25, 2026)

### Added
* Sanwa Metallic Edition Pushbuttons: Added 30mm Sanwa OBSF-30 metallic series, Seimitsu PS-14-GN metallic, and Crown SDB-202 metallic pushbuttons with electroplated finishes.
* WS2812B RGB Telemetry Matrix Displays: Added 4x12, 8x8, and 16x16 LED matrix modules with live 5V electrical current budget modeling.
* Auxiliary 5V Power Injection Standard: Added auxiliary power injection configuration to support high-density LED arrays and external powered hubs without controller disconnects.
* Ferrari Corsa Gloss Red Acrylic: Added high-gloss mirror-finish racing red cast acrylic to the material catalog as the default rear enclosure plate.
* Parametric Captive T-Nut Controls: Added custom setback margins and per-axis count selectors with automatic corner joint clearance recommendations.
* Manufacturing-Aware Legend Renderers: Added distinct visual representations for laser surface etching, CNC V-carved groove engraving, and 3D print tactile embossed lettering.
* Mechanical Switch Acoustics: Added procedural sound simulations for Cherry MX Blue clicky, Cherry MX Red linear, Cherry MX Brown tactile, and Topre capacitive switch press profiles.

### Improved
* Corner Finger Joint Flush Alignment: Refined interlocking finger tabs so all 4 corners fit flush against adjacent box walls.
* Default Studio Configuration: Updated demo GT3 enclosure to 240mm x 180mm with 30mm metallic arcade buttons, shift light bar, laser process preset, and interactive DRC power validation.
* Material Palette Filtering: Material selectors now strictly display materials compatible with the active manufacturing machine (Laser, CNC, or 3D Print).
* DRC Contextual Auto-Fixes: Power budget, faceplate thickness, laser bed overflow, and VESA pattern issues now trigger specific, context-appropriate actions.

---

## [v0.4.0] (October 25, 2026)

### Added
* Additive Unibody Enclosure Topologies: Added Monolithic Rear Tub, Monolithic Front Bezel, and Dual-Open Sleeve Frame for 3D printing and CNC milling.
* Additive Fastener Systems: Added support for captive hex nut pockets, M3 brass heat-set threaded inserts, and direct plastic thread-forming screws.
* Fabrication Workflow Selector: Added top-level process toggle (3D Print, Laser Cut, CNC Milled) with automated material and machine presets.
* Binary STL Exporter: Added client-side export for watertight, manifold Binary STL meshes for 3D printing.

### Improved
* Mounting Flange Alignment: Refined mounting ear filleting to ensure flush boundary collinearity.
* Multi-Topology DRC: Synchronized collision detection and internal depth checking across all sheet box and unibody models.

---

## [v0.3.0] (October 25, 2026)

### Added
* Parametric Aircraft Missile Safety Cover: Added realistic multi-part safety toggle cover with protective canopy and bat lever.
* Exploded View Animation: Added continuous animation loop that sweeps explosion progress and dynamically rotates the missile canopy open.
* Zero-Latency Web Audio Engine: Procedural sound synthesis engine reproducing tactile switch actuation, microswitch springs, and detent clicks.
* Interactive 3D Control Actuation: Click-to-actuate 3D controls with persistent toggle states and illumination.

### Improved
* Exploded View Kinematics: Smooth angular opening synchronized with exploded view expansion.

---

## [v0.2.0] (October 25, 2026)

### Added
* Photorealistic CC0 PBR Materials: 1K photographic textures for Baltic Birch, American Walnut, White Oak, Cherry Veneer, 3K Carbon Fiber Twill, and Brushed Aluminum.
* Full-Gamut Button Colors & Metallic Finishes: Dynamic color and electroplated metallic finishes across button bodies, plungers, and LED halos.
* Box Frame Laser Cut Sheets: Multi-panel 2D cut sheet generation with isolated legend etches and kerf offsets.
* Parametric Corner Geometry: Configurable square corners and rounded fillets.
* 3-Tab Studio Inspector Dock: Unified sidebar for Design Rule Checks (DRC), Bill of Materials (BOM), and Component Library.
* Magnetic Snap Mounting Ears: 8020 aluminum extrusion mounting flanges with edge snap alignment.

---

## [v0.1.0] (October 24, 2026)

### Added
* Parametric Sim Rig Button Box Studio: Interactive 2D vector CAD canvas and 3D WebGL viewport for designing bespoke sim racing button boxes.
* Arcade and Industrial Component Library: Parametric footprints for Sanwa OBSF series, Seimitsu, heavy-duty toggle switches, rotary encoders, missile safety switches, and OLED telemetry displays.
* Live Design Rule Check (DRC) Engine: Real-time validation for component collisions, keep-out boundary margins, faceplate thickness compatibility, and machine bed limits.
* Electrical and GPIO Budgeting Engine: Dynamic electrical analysis calculating digital inputs, rotary encoder pulse channels, matrix diode grids, and 5V USB power consumption.
* Fabrication Faceplate Export: Production-grade vector SVG faceplate exports with configurable beam kerf compensation, raster text engraving, and precision inner and outer cut layers.
* Microcontroller Wiring Companion: Interactive physical pinout checklist and rear wiring schematics supporting Raspberry Pi RP2040, Arduino Pro Micro, and Zero-Delay USB encoders.

---

*For inquiries and custom enterprise presets, visit [switchrigapp.com](https://switchrigapp.com).*
