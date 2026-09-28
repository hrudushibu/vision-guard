# Vision Guard — AI Agent Rules

This file provides guidance to AI agents working on Vision Guard, a computer-vision security framework.

## 🎯 Project Context

**Vision Guard** uses computer vision and AI to detect physical security events from video. You're building a system that can monitor camera feeds and identify intrusions, restricted-area access, and unusual activity.

- **Repository**: [https://github.com/hrudushibu/vision-guard](https://github.com/hrudushibu/vision-guard)
- **License**: Apache-2.0
- **Contact**: [hrudushibu.tech@gmail.com](mailto:hrudushibu.tech@gmail.com)

## 🚧 Development Stage

**Early Development** — Computer vision pipeline, detection algorithms, and video processing approach are being designed. Implementation is in progress.

## 📹 Core Principles

### Real-Time Performance
Video analysis must run in real-time for live monitoring. Optimize for speed without sacrificing accuracy.

### Privacy by Design
Video contains sensitive information. Implement privacy controls like face blurring and zone masking.

### Explainable Detections
When an event is detected, show why. Annotate the video to highlight what triggered the alert.

### Extensible Pipeline
Different environments need different detectors. Build a plugin architecture for custom detection logic.

## 💻 Tech Stack

- **Next.js 16** with App Router
- **React 19** with Server Components
- **TypeScript 5** in strict mode
- **Tailwind CSS 4** for styling
- **shadcn/ui** for components

## 📂 Current Project Structure

```
app/                  # Next.js App Router pages
components/
  app/                # App-wide layouts
  console/            # Console-specific UI
  ui/                 # Base UI primitives
lib/                  # Shared utilities
```

**Note**: Computer vision and detection folders will be added as development progresses.

## 🚨 Security & Privacy Considerations

### Video Data Privacy
Video surveillance is sensitive. Implement access controls, retention policies, and privacy zones.

### False Positive Management
Balance detection sensitivity to minimize false alarms while catching real events.

### Performance Under Load
Multiple camera feeds require significant processing power. Design for horizontal scaling.

---

<!-- BEGIN:nextjs-agent-rules -->

# This is NOT the Next.js you know

This version has breaking changes — APIs, conventions, and file structure may all differ from your training data. Read the relevant guide in `node_modules/next/dist/docs/` (resolved from this file's directory; in monorepos the `next` package may not be visible from the repo root) before writing any code. Heed deprecation notices.

This block is written and re-added by `next dev` — verify at `node_modules/next/dist/server/lib/generate-agent-files.js`. Removing it from a diff only re-creates the uncommitted change; committing it with your work keeps the tree clean.

<!-- END:nextjs-agent-rules -->
