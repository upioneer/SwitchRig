# SwitchRig Button Box Studio Changelog

All notable changes, manufacturing updates, and component catalog additions to SwitchRig Button Box Studio are documented in this file.

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

*For inquiries and custom enterprise presets, visit [switchrigapp.com](https://switchrigapp.com).*
