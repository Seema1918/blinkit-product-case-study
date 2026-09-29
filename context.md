# Project Context

## Working Title

**Hyperlocal Velocity** - a quick-commerce delivery experience for making peak-hour delivery promises more accurate, transparent, and actionable.

## Source of Truth

The initial product direction comes from `PRD- Blinkit.pdf` and the accompanying Stitch prototypes in `Prototype/`. The repository is a portfolio project and product-design exploration; it is not affiliated with or endorsed by Blinkit.

## Problem

During peak-demand periods, customers can receive an ETA that no longer reflects store workload, rider availability, traffic, or building-level delivery friction. Unexpected delays create anxiety, late-delivery cancellations, and reduced trust in the service.

The experience should make the promise useful even when conditions change: provide a credible ETA, explain what affects it, and communicate a revised promise before the original window is missed.

## Product Goal

Improve confidence in peak-hour quick-commerce delivery by combining:

1. Dynamic ETA prediction based on live operational signals.
2. Proactive delay alerts with a revised ETA and a clear reason.
3. Scheduled delivery slots for customers who prefer predictability over speed.

## Primary User

An urban quick-commerce customer ordering groceries during a high-demand period. They value speed, but they value a trustworthy promise and timely updates more than an optimistic countdown.

### User needs

- Know when the order is likely to arrive.
- Understand whether the promise is still on track.
- Hear about a likely delay before it becomes a missed promise.
- Choose a predictable slot when instant delivery is uncertain.
- Contact support or the delivery partner without losing order context.

## Key Journey

1. **Discover:** Browse products while seeing the current delivery promise and local operating conditions.
2. **Choose:** Review the cart, inspect the ETA explanation, and select express delivery or a scheduled slot.
3. **Track:** Follow store preparation, rider dispatch, route progress, and the reason behind the current ETA.
4. **Recover:** Receive an early delay alert with the original ETA, revised ETA, cause, and available support or compensation.
5. **Learn:** Evaluate the delivery experience through on-time performance and customer feedback.

## Product Scope

### In scope

- Home/discovery experience with dynamic ETA context.
- Cart and checkout with ETA transparency and delivery-slot selection.
- Live order tracking with milestones, route context, rider details, and ETA signals.
- Proactive delay notification with revised ETA and acknowledgement.
- Responsive web and mobile layouts.
- Simulated operational data for a convincing portfolio prototype.

### Out of scope

- Inventory or product-availability improvements.
- Redesigning the delivery network or dark-store operations.
- Address management as a standalone product area.
- Real payments, real-time maps, production notifications, or live rider data.

## Success Measures

### North-star metric

- Orders delivered within the promised delivery time.

### Supporting measures

- Orders delivered close to the promised ETA.
- Orders delivered after the promised ETA.
- Cancellations caused by late delivery.
- Time between detecting a likely delay and notifying the customer.
- Difference between predicted ETA and actual delivery time.

The prototype should make these measures visible in the product story, while clearly labeling any sample values as simulated.

## Design Direction

The existing `Hyperlocal Velocity` design system describes the intended visual language:

- Tactile modern utility: dense, scannable, touch-friendly modules.
- Primary green for progress, purchase, and operational confidence.
- Yellow/amber for peak-demand and proactive delay states, avoiding alarmist red.
- Plus Jakarta Sans with strong numeric hierarchy for prices and ETAs.
- Four-signal ETA explanation: store queue, picking, rider transit, and gate buffer.
- Responsive layouts with 44px minimum touch targets and mobile safe-area support.

## Assumptions and Open Questions

- The first implementation can use deterministic mock telemetry and simulated time progression.
- ETA calculation is initially a transparent rules-based model, not a trained machine-learning model.
- The portfolio version should demonstrate the customer experience and system thinking without implying access to Blinkit's internal data.
- Before production work, validate signal quality, notification timing, compensation policy, location privacy, and the definition of "close to promised ETA" with stakeholders.
