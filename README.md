# FlapperSurveillanceVan7
I originally intended to become a marine biologist studying sharks. These days, I spend more time watching the birds visiting a backyard feeder instead.

This project developed from wanting a better way to observe and document activity at the feeder while also exploring motion detection, camera setup, environmental troubleshooting, and incremental computer vision workflows using consumer hardware and real-world constraints.
The project also intends to illustrate how similar monitoring and identification challenges may appear in broader wildlife or environmental observation contexts, where behavior, lighting, movement, and capture conditions are rarely ideal.

## Project Intro
### Project Goals
Detect meaningful movement at the feeder and capture useful recordings/events without excessive false positives.
Examples include:
- birds landing on the feeder
- larger birds moving the feeder
- possible nighttime visitors (such as possums)


## Why does this project exist?
This project is intentionally grounded in real-world support engineering thinking.

The goal is not simply "build AI," but to work through:
- hardware constraints
- deployment tradeoffs
- troubleshooting
- environmental unpredictability
- storage considerations
- iterative improvement
- and practical user-facing problem solving

The project reflects how real customers approach technical problems:
starting with imperfect hardware, evolving requirements, and practical limitations.


## Existing Hardware Options
### Creative Webcam
Pros:
- Continuous computer connection
- Easy live monitoring
- Simple development/testing workflow

Limitations:
- Requires a dedicated running computer
- Requires active storage management
- Outdoor positioning may be difficult

---

### Early Model GoPro
Pros:
- Self-contained recording
- Flexible outdoor positioning
- Good image quality potential

Limitations:
- Requires manual retrieval/download
- Positioning experimentation required
- Battery/runtime constraints

---

### Spare iPhone 14
Pros:
- High-quality camera
- Local recording directly to device
- Flexible mounting options
- Potential for app-based automation later

Limitations:
- Likely requires tripod/mount adapter
- Battery management considerations
- Storage usage on device

Current likely direction:
Use the iPhone as the primary outdoor camera platform during early experimentation.

---

## Detection Strategy
### Phase 1 — Motion Detection
Start with basic motion/event detection to verify:
- camera positioning
- lighting conditions
- feeder visibility
- recording reliability

This phase intentionally prioritizes operational stability over AI complexity.

---

### Phase 2 — Motion Tuning
Reduce false positives by:
- filtering small environmental movement
- tuning sensitivity thresholds
- focusing on feeder-area motion
- differentiating between feeder sway and actual visitors

---

### Phase 3 — Night Observation
Explore nighttime monitoring possibilities:
- low-light recording
- infrared/night-vision options
- detecting nocturnal visitors such as possums

---

## Future AI Possibilities

Potential future integration ideas:
- bird presence detection
- species classification
- event summaries
- visitor statistics
- cloud-hosted inference pipelines
- Roboflow workflow experimentation


## Operational Constraints
The project operates under a number of practical and environmental constraints that may affect observation quality and consistency.

Variables such as:
- food type
- weather conditions
- feeder movement from wind or larger birds
- lighting changes throughout the day
- seasonal visitor patterns
- temporary camera placement
- battery/runtime limitations
- and storage availability

may all influence what activity is captured and how reliable the resulting footage becomes.

The project also intentionally relies on accessible consumer hardware rather than specialized monitoring equipment, requiring iterative adjustments and practical compromise during setup and testing.


## Current status
**Project stage: Feasibility review and early planning**

Current status:
- Existing feeder already active
- Multiple camera options available
- No production code written yet
- No camera tests completed yet
- Initial workflow and architecture planning in progress

## Planned next steps

The following list is intended as an initial working checklist and will likely evolve as testing and observation continue.

- Create a basic materials list for the first test setup
- Gather available camera, mounting, power, and storage items
- Check that equipment is working, including but not limited to:
  - batteries charged
  - adapters fit
  - camera stance is stable
  - feeder is clearly in frame
- Prepare the feeder with the selected seed/food
- Run a short test recording
- Review the footage for visibility, motion, lighting, and feeder movement
- Step back and reassess the setup, assumptions, and recording quality before expanding the project further
- Adjust setup based on findings
- Run a longer live test/capture once the basic setup is reliable
