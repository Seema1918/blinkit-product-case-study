# Blinkit Product Case Study

**A portfolio exploration of trustworthy delivery promises during peak-hour quick commerce.**

Hyperlocal Velocity explores what happens when a 10-minute delivery promise meets real operational conditions: dark-store workload, rider availability, traffic, and the last few meters to a customer's door. Instead of hiding uncertainty behind a single countdown, the experience makes the ETA understandable, updates it early, and gives the customer a predictable alternative.

> This is an independent portfolio project inspired by a Blinkit delivery experience brief. It is not affiliated with or endorsed by Blinkit. All operational data shown in the prototypes is simulated.

## The Product Story

The project follows one order across five connected moments:

- **Discovery:** a live delivery promise and local peak-demand context.
- **Checkout:** an explainable ETA with express and scheduled delivery choices.
- **Live tracking:** store, rider, route, and milestone telemetry in one view.
- **Proactive delay:** an early notification with the original ETA, revised ETA, reason, and support path.
- **Hyperlocal system:** a shared visual language for speed, trust, and operational clarity.

The core product bet is simple: a revised promise communicated early is more trustworthy than an optimistic promise that fails silently.

## Screen Previews

| Web discovery | Mobile discovery |
| --- | --- |
| ![Web discovery screen](Prototype/Web%20Screens/Website%20screens/stitch_predictive_quick_commerce_delivery_experience/home_discovery_dynamic_eta/screen.png) | ![Mobile discovery screen](Prototype/Mobile%20screens/Mobile%20Screens/mobile_home_discovery_dynamic_eta/screen.png) |

| Proactive delay alert |
| --- |
| ![Web proactive delay alert](Prototype/Web%20Screens/Website%20screens/stitch_predictive_quick_commerce_delivery_experience/proactive_delay_alert_updated_eta/screen.png) |

## Current Prototype

The repository currently contains responsive HTML prototypes for web and mobile:

- Web discovery and dynamic ETA
- Web cart, checkout, and slot selection
- Web live order tracking
- Web proactive delay alert and updated ETA
- Matching mobile discovery, checkout, live tracking, and delay-alert flows
- Shared `Hyperlocal Velocity` design system documentation

Open any linked `code.html` file to inspect a screen directly in a browser. The HTML files are self-contained prototypes; they are intentionally kept close to the original design exploration so the interaction decisions remain easy to review.

### Mobile screens

- [Home discovery and dynamic ETA](Prototype/Mobile%20screens/Mobile%20Screens/mobile_home_discovery_dynamic_eta/code.html)
- [Cart, checkout, and slot selection](Prototype/Mobile%20screens/Mobile%20Screens/mobile_cart_checkout_slot_selection/code.html)
- [Real-time live order tracking](Prototype/Mobile%20screens/Mobile%20Screens/mobile_real_time_live_order_tracking/code.html)
- [Proactive delay alert and updated ETA](Prototype/Mobile%20screens/Mobile%20Screens/mobile_proactive_delay_alert_updated_eta/code.html)
- [Mobile design system](Prototype/Mobile%20screens/Mobile%20Screens/hyperlocal_velocity/DESIGN.md)

### Web screens

- [Home discovery and dynamic ETA](Prototype/Web%20Screens/Website%20screens/stitch_predictive_quick_commerce_delivery_experience/home_discovery_dynamic_eta/code.html)
- [Cart, checkout, and slot selection](Prototype/Web%20Screens/Website%20screens/stitch_predictive_quick_commerce_delivery_experience/cart_checkout_slot_selection/code.html)
- [Real-time live order tracking](Prototype/Web%20Screens/Website%20screens/stitch_predictive_quick_commerce_delivery_experience/real_time_live_order_tracking/code.html)
- [Proactive delay alert and updated ETA](Prototype/Web%20Screens/Website%20screens/stitch_predictive_quick_commerce_delivery_experience/proactive_delay_alert_updated_eta/code.html)
- [Web design system](Prototype/Web%20Screens/Website%20screens/stitch_predictive_quick_commerce_delivery_experience/hyperlocal_velocity/DESIGN.md)

## Repository Map

```text
.
├── context.md                 # Product context, scope, users, and success measures
├── plan.md                    # Implementation phases and acceptance scenarios
└── Prototype/
    ├── Mobile screens/
    └── Web Screens/
```

## Run Locally

The current screens are self-contained HTML files and use CDN-hosted Tailwind CSS, fonts, icons, and prototype imagery.

1. Open any `code.html` file from `Prototype/` in a browser, or serve the repository with a local static server.
2. For a more reliable browser experience, run a static server from the repository root, for example:

```bash
npx serve .
```

There is no build step or backend in the current prototype. The planned interactive implementation is documented in [plan.md](plan.md).

## Push to GitHub

The `main` branch is connected to the configured `origin` remote. From this repository folder, review and publish the project files:

```bash
git add .gitignore .gitattributes README.md context.md plan.md Prototype/
git status --short
git commit -m "Add Hyperlocal Velocity portfolio prototype"
git push origin main
```

The original brief is intentionally excluded. The prototype uses external font, icon, and image URLs; review those dependencies before publishing.

## Design Notes

The interface uses the existing Hyperlocal Velocity system: tactile utility, compact operational modules, strong numeric hierarchy, green progress states, and calm amber delay communication. The design system is documented in the `hyperlocal_velocity/DESIGN.md` files inside the web and mobile prototype areas.

## Product Metrics

The PRD prioritizes:

- Orders delivered within the promised delivery time.
- The gap between predicted and actual delivery time.
- Orders delivered after the promised ETA.
- Cancellations caused by late delivery.

The prototype demonstrates the information and interaction model for improving these outcomes; it does not claim to measure them with live production data.

## What Comes Next

- Consolidate the prototype flows around one shared simulated order state.
- Implement dynamic ETA transitions and proactive delay triggering.
- Add focused accessibility and responsive testing.
- Publish a short case-study walkthrough with screenshots, tradeoffs, and limitations.

## Documentation

- [Project context](context.md)
- [Implementation plan](plan.md)
