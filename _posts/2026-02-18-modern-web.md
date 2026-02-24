---
layout: default
title: "Design Engineer Showcase: Diny"
description: "As the Founding Design Engineer for Diny, I owned the product experience from a blank canvas to a fully deployed production environment."
date: 2026-02-18
tags: [web, development, technology, design]
slug: diny
---
# Design Engineer Showcase: Diny

**A next-generation dining and ordering platform.**

*Co-Founder & Founding Design Engineer •* End-to-End (Ideation, UI/UX Design, Architecture, Production Implementation)

As the Founding Design Engineer for Diny, I owned the product experience from a blank canvas to a fully deployed production environment. My core philosophy for this project was to blur the lines between high-fidelity UI design and hardcore performance engineering. The result is a frictionless, visually rich, and deeply optimized ordering platform that respects the user's time and device capabilities.

Below is a deep dive into the core experiences I designed and built.

<video src="demos/full-experience.mp4" controls width="640" autoplay loop muted></video>

---

## 1. The Search Experience: Fluidity Meets Performance

<video src="demos/search.mp4" controls width="640" autoplay loop muted></video>

The search interface is the front door to Diny, designed to give users all necessary information at a glance (prep time, distance, available services, and cuisine type) without overwhelming them.

- **Visual Architecture:** Restaurant cards feature unique covers that fluidly transition into a blurred background, establishing a distinct visual identity for every venue.
- **Custom Shared Transitions:** I implemented custom spring animations to drive fluid, smooth content zoom transitions.
- **Deep Performance Optimization:** Achieving 60FPS during complex transitions on low-end Android devices was a primary technical challenge. I built custom render pipelines using advanced memoization, virtualization, and lazy execution logic, ultimately outperforming native Android page transitions.
- **Micro-Interactions:** Perfected search bar layer manipulation (surpassing the UX of top-tier marketplaces like Airbnb or the App Store) and implemented custom bidirectional swipe-to-close gestures, grounding the app in highly engaging, best-in-class tactile patterns.

---

## 2. Restaurant View: Edge-to-Edge Immersion

<video src="demos/place.mp4" controls width="640" autoplay loop muted></video>

Navigating from the search screen to the restaurant details feels less like a page load and more like a camera zooming into the venue.

- **Continuous Context:** The unique place blueprint extends into a full edge-to-edge experience, seamlessly transitioning into the menu section.
- **Sticky Information:** Crucial data—like time-to-ready, distance, and the search bar—remains pinned and visible. Top-bar animations dynamically reveal contextual content as the user scrolls.
- **Conversion-First Menu UX:** The menu structure prioritizes the dish's visual appeal at the very top. By giving users immediate visual understanding and a frictionless one-tap "Add to Basket" action, the design actively drives conversion.

---

## 3. Synchronized Menu Navigation

<video src="demos/sections.mov" controls width="640" autoplay loop muted></video>
<video src="demos/sections2.mov" controls width="640" autoplay loop muted></video>
<video src="demos/section3.mp4" controls width="640" autoplay loop muted></video>

Menu navigation is historically clunky in the food delivery industry. I engineered a multi-directional navigation system that feels magical and requires zero cognitive load.

- **Bidirectional Sync:** Scrolling the content automatically updates the selected section pill, and tapping a section smoothly scrolls the content to the right place.
- **Swipeable Categories:** Users can simply scroll horizontally through the menu sections, and the content will auto-align without requiring multiple distinct gestures.
- **Polished Kinematics:** Powered by perfectly tuned spring animations, the experience is optimized to run synchronously and flawlessly, regardless of menu size.

---

## 4. Frictionless Selection

<video src="demos/menu.mov" controls width="640" autoplay loop muted></video>
<video src="demos/order2.mov" controls width="640" autoplay loop muted></video>

In Diny, we believe software should give you your time back. The checkout flow starts with a radical approach to item selection: it takes only one tap.

- **Fluid Quantity Controls:** Adding an item immediately triggers a fluid animation that expands the component to reveal quantity controls (+ / -).
- **Instant Discovery:** Multiple item variants are easily discoverable and viewable without drilling down into new screens, accelerating the decision-making process.
- **Engineering Resilience:** To prevent API overloads from rapid tapping, I engineered a resilient queuing behavior. Loaders are elegantly embedded directly into the action buttons (plus/minus) to provide instant feedback while safely handling backend requests. This complex animation state was thoroughly optimized to play nicely with list virtualization.

---

## 5. Contextual Checkout Flow

<video src="demos/order.mp4"  controls width="640" autoplay loop muted></video>
<video src="demos/order3.mov" controls width="640" autoplay loop muted></video>

The checkout process was designed to never interrupt the user's context. Instead of bouncing the user to a new page, checkout happens in a highly polished bottom sheet.

- **Frosted Glass & Context:** A frosted glass background keeps the restaurant context visually present while the user reviews their order.
- **Optimistic UI:** Price counters and item additions update optimistically, providing instantaneous feedback. Adding an item triggers a satisfying, springy slide-in transition within the sheet.
- **Two-Step Checkout:** By integrating Apple Pay, the entire flow is reduced to just two steps: *Add* and *Pay*.
- **Persistent Live State:** Post-purchase, real-time updates are delivered via a persistent bottom pill that follows the user throughout the app, offering reassurance without interrupting further exploration.

---

## 6. Eatfeed: Immersive Discovery

<video src="demos/eatfeed.mp4" controls width="640" autoplay loop muted></video>

Borrowing high-engagement paradigms from social media, I introduced a swipe-based food selection experience to the dining industry.

- **Zoom-to-Feed:** Leveraging the same smooth transition logic from the search page, a standard list of dishes can transform into a swipeable, full-screen food feed.
- **Edge-to-Edge Exploration:** Users can navigate visually rich, full-screen dish images with simple swipes, completely eliminating the annoying "go back" interaction loop.
- **Quick Actions:** Even in this immersive mode, users have instant access to add items, view their cart, and edit their order on the fly.


