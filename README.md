Old School Boxing & Fitness Center (obc) Website 
Project Version: 1.2.0

Once the server has started, open a web browser and navigate to:
http://localhost:8080


This project is the official website for Old School Boxing & Fitness, designed for a modern aesthetic using a dark, high-contrast, and glassmorphism-inspired UI. The goal is to convey discipline, strength, and community.

Technology Stack
Frontend: HTML5, Tailwind CSS (loaded via CDN)

Styling: Custom CSS for Glassmorphism effects and color variables.

Forms/CTA: Integrated with Formspree (for general submissions) and MailerLite (for pop-up lead capture).

Icons: Font Awesome (CDN).

Design & Styling System
The entire website follows a consistent, high-impact design language:

Feature

Description

Tailwind Classes/Notes

Background

Smooth dark gradient

bg-gradient-to-br from-black via-gray-900 to-black

Glassmorphism

Used for all cards, navbar, and primary sections.

bg-white/10 backdrop-blur-lg border border-white/20 shadow-md

Primary Color

Red accent for headings and buttons.

text-red-600, bg-red-600

Typography

Sans-serif (system default/Inter), high contrast.

text-white, text-gray-200

CTA Buttons

Red, rounded, bold text, subtle hover glow/shadow.

bg-red-600 hover:bg-red-700 py-3 px-8 rounded-xl

Alignment

Content within pricing cards is aligned vertically using Flexbox (flex flex-col justify-between) for consistent button placement.



Page Breakdown
The site consists of five main pages, all sharing the unified design system:

1. index.html (Home Page)

Hero: Features a high-contrast title and gym image.

Features Section ("Why Choose Us"): Three glass cards with bold titles and stylized, dedicated icons (Diamond for Elite Coaches, Lightning Bolt for Intensity, Users for Community).

Modal Pop-up: A prominent, full-screen pop-up modal triggers automatically to capture emails for a free session using MailerLite.

2. about.html (About Page)

Mission & Vision: Presented side-by-side in two equal-height glass cards, featuring bulleted lists for clarity and strong red headings.

Coaches Section: Displays profiles of three coaches with circular images and brief descriptions.

3. schedule.html (Schedule Page)

Layout: Uses a highly streamlined, Notion-style table grid for weekly classes.

Structure: Classes are grouped into columns (Mon - Fri and Sat / Sun) for easy digestion.

Alignment: The schedule table and the bottom CTA card are perfectly aligned using max-w-4xl mx-auto.

4. pricing.html (Membership Page)

Core Plans: Three vertically aligned cards (Month-to-Month, 6-Month, 1-Year) ensuring buttons are horizontally aligned using Flexbox.

Includes "Popular" (Red) and "Best Value" (Yellow/Black) flags.

Add-Ons: Dedicated section for specialty plans and passes (Children's, One-on-One, Passes dropdown).

5. enroll.html (Signup Page)

Layout: Divided into a primary Form Card (left) and a "What to Bring" Info Card (right).

Form Functionality: Submits data directly to Formspree (https://formspree.io/f/xqayknwq).

Custom Select: Features a custom-styled dropdown menu for "Experience" with a solid dark background for enhanced legibility.

Getting Started
Clone the Repository: (Assume standard git cloning steps here)

Open Files: Since no compilation is needed, simply open index.html in your web browser to view the site.

Ensure Connectivity: The site relies on external CDNs (Tailwind CSS, Font Awesome) and third-party services (MailerLite, Formspree). Ensure your environment allows these external scripts to run.

Form and External Service Details
Main Contact Forms (enroll.html): Uses the Formspree endpoint https://formspree.io/f/xqayknwq.

Lead Capture Modal (index.html): Uses the MailerLite Universal script and is configured to trigger form ID OAsLDy after 4-6 seconds of page load.