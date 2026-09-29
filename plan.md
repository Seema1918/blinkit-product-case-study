# Project Plan

## Outcome

Turn the existing responsive HTML prototypes into a focused, explainable portfolio project that demonstrates how a quick-commerce experience can handle peak-hour uncertainty without hiding it from the customer.

## Guiding Principles

- Build the highest-priority trust moment first: proactive delay communication.
- Keep every ETA explainable through observable signals.
- Treat the promise as a state that can change, not a static marketing number.
- Use simulated data honestly and make the simulation easy to replace.
- Preserve the existing Hyperlocal Velocity design language across web and mobile.

## Phases

### Phase 0 - Repository foundation

- Add project context, plan, and portfolio README.
- Consolidate the source PRD and prototype links in the project documentation.
- Decide whether the final build will remain static HTML or move to a small frontend application.

**Exit criteria:** A new contributor can understand the problem, scope, prototype surfaces, and next implementation step from the repository root.

### Phase 1 - Prototype audit and shared model

- Inventory the five core surfaces: discovery, checkout, live tracking, proactive delay alert, and hyperlocal velocity/design system.
- Identify repeated tokens, header patterns, ETA components, timeline states, and responsive behavior.
- Define shared mock entities: customer, order, basket, dark store, rider, route, ETA signals, and delay event.
- Normalize sample values so the same order tells one consistent story across screens.

**Exit criteria:** All screens can describe the same order lifecycle and use one documented mock data shape.

### Phase 2 - Interactive experience

- Add a shared simulated clock and order-state transitions.
- Make ETA breakdown details expandable and readable on mobile.
- Support express versus scheduled slot selection in checkout.
- Add cart quantity interactions and preserve the selected delivery mode.
- Move the order through packed, dispatched, delayed, and delivered states.
- Trigger the proactive alert before the original ETA and show the revised promise.
- Make acknowledgement, support, rider contact, and order-summary interactions explicit.

**Exit criteria:** A reviewer can complete one end-to-end scenario without dead links or unexplained state changes.

### Phase 3 - Reliability and accessibility pass

- Test responsive behavior at representative mobile, tablet, and desktop widths.
- Check keyboard navigation, focus visibility, semantic labels, contrast, and reduced-motion behavior.
- Ensure changing ETA values do not cause layout shifts.
- Remove production-looking claims from simulated data or label them clearly.
- Verify that third-party image and font dependencies have a suitable portfolio fallback.

**Exit criteria:** The primary journey is usable with keyboard and touch, and the main states remain legible across supported viewports.

### Phase 4 - Portfolio presentation

- Add screenshots or a short walkthrough of the main journey.
- Document the problem, prioritization, design decisions, tradeoffs, and limitations.
- Add a concise local run guide and project structure overview.
- Include a short "what I would build next" section.

**Exit criteria:** A hiring manager can understand the product decision, inspect the experience, and run the project without prior context.

## Recommended Implementation Shape

Start with the existing HTML/CSS/JavaScript prototypes. If state sharing across surfaces becomes difficult, migrate only the interactive shell to a small component-based frontend and keep the design tokens and content structure intact. Avoid introducing a backend until the customer journey and simulation are stable.

### Suggested domain modules

- `eta`: signal inputs, ETA calculation, confidence, and revised promises.
- `order`: order lifecycle and milestone transitions.
- `delivery-slots`: express and scheduled options.
- `notifications`: proactive delay event and acknowledgement state.
- `telemetry`: deterministic mock store, traffic, rider, and gate data.
- `ui`: shared ETA, status, timeline, slot, cart, and support components.

## Acceptance Scenarios

1. A customer opens discovery during peak demand and sees a current delivery promise.
2. A customer opens checkout and can inspect the four ETA signals.
3. A customer can choose fastest delivery or a future slot, and the choice is visible in the order summary.
4. A live order shows milestones, rider context, route progress, and the current ETA.
5. A simulated store or traffic change revises the ETA within a few seconds.
6. The customer receives a proactive delay state before the original promise expires.
7. The delay state shows original ETA, revised ETA, cause, and a support path.
8. All primary actions remain usable on mobile and desktop.

## Risks and Mitigations

| Risk | Mitigation |
| --- | --- |
| Static screens tell conflicting stories | Use one shared mock order and a small state machine. |
| ETA appears arbitrary | Show the four signal inputs and document the calculation. |
| Delay alert creates anxiety | Use calm amber semantics, early notice, and a concrete revised promise. |
| Portfolio readers mistake sample data for production data | Label simulated telemetry and list production limitations. |
| Scope expands into a full commerce platform | Keep inventory, payments, and network redesign explicitly out of scope. |
