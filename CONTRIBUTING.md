# Contributing to SwitchRig App

Thank you for contributing to SwitchRig App. This public repository serves as the community hub for bug reporting, feature proposals, and hardware footprint requests.

---

## How to Contribute

### 1. Reporting Bugs

If you encounter an issue with CAD export, collision calculations, browser rendering, or user interface controls:

* Check existing [GitHub Issues](../../issues) to avoid duplicates.
* Use the [Bug Report Template](../../issues/new?template=bug_report.yml).
* Include clear details:
  * Operating System and Web Browser (Chrome, Firefox, Safari, Edge).
  * Active Machine Profile and Process (Laser Cut, CNC, 3D Print).
  * Enclosure Dimensions and Fastening Mode.
  * Steps to reproduce the issue.
  * Screenshots, exported SVG/DXF files, or browser console errors if applicable.

---

### 2. Proposing Studio Features & Tools

Have an idea for a layout tool, parametric joint option, export format, or DRC rule?

* Check existing [GitHub Issues](../../issues) to see if a similar proposal is already being discussed.
* Use the [Feature Proposal Template](../../issues/new?template=feature_request.yml).
* Describe the specific design limitation, your proposed workflow enhancement, and any relevant CAD mockups or sketches.

---

### 3. Requesting New Components & Hardware

We regularly expand the component library with authentic sim racing and arcade hardware footprints. When requesting a new switch, button, display, or encoder, please use the [Component Request Template](../../issues/new?template=component_request.yml) and provide as much technical specification data as possible:

* **Manufacturer & Model:** (e.g. Sanwa OBSN-30, NKK S-302T, Bourns PEC11R)
* **Category:** (Pushbutton, Rotary Encoder, Toggle Switch, Display, Key Switch)
* **Cutout Shape & Dimensions:** Round diameter (mm) or rectangular width $\times$ height (mm).
* **Keep-Out Envelope:** Maximum exterior flange diameter / bezel envelope (mm).
* **Under-Panel Internal Depth:** Clearance needed from back of faceplate to terminal tips (mm).
* **Mounting Style:** Snap-in retaining clips or threaded barrel with retaining nut.
* **Max Panel Thickness:** Maximum faceplate thickness supported by the component (mm).
* **Terminal Type:** Quick-disconnect spade (2.8mm, 4.8mm, 6.3mm), solder lugs, or pin headers.
* **Electrical Load:** Typical 5V current draw (mA) if illuminated or containing microcontrollers.
* **Manufacturer Datasheet / Technical Drawing:** Link to manufacturer drawing or PDF.

---

### 4. Requesting Machine Presets & Materials

To request support for a specific laser cutter, CNC router, 3D printer, or manufacturing material:

* Use the [Machine & Material Request Template](../../issues/new?template=machine_material_request.yml).
* For machines, provide:
  * Machine make and model.
  * Fabrication class (CO2 Laser, Diode Laser, Fiber Laser, CNC Router, 3D Printer).
  * Usable working bed envelope ($X \times Y$ dimensions in mm).
  * Typical kerf width or recommended tool bit diameter.
* For materials, provide:
  * Material family (Cast Acrylic, Plywood, Solid Hardwood, Carbon Fiber Composite, Anodized Aluminum, 3D Filament).
  * Nominal thicknesses commonly available.
  * Typical laser cutting / CNC machining compatibility considerations.

---

## Community Guidelines

* Please keep discussions respectful, constructive, and focused on physical fabrication and sim racing engineering.
* For issues with your local hardware (e.g. laser power calibration, CNC feeds and speeds, wiring soldering), provide context so community members can assist effectively.
