# DMI Portfolio Website (Static HTML/CSS)

This repository contains a clean, professional-looking **static portfolio website** used in **DevOps Micro Internship (DMI)** Week 1 to practice:
- Linux basics
- Nginx hosting
- Deployment proof / ownership
- Production-style checks

✅ Students deploy this website on an Ubuntu VM using Nginx and keep it live for 24 hours.

---

## Who is this for?
- DMI students (beginner → intermediate)
- Anyone learning how to host a static site with Nginx on Linux

---

## What you will build
A portfolio-style website hosted on:
- **Ubuntu VM**
- **Nginx**
- Accessible via: `http://<public-ip>`

---

## Mandatory Ownership Proof (DMI Rule)
Before you deploy, you MUST edit the footer and add your details:

Original:

```html
<p>Crafted with <span>cloud</span> excellence by Pravin Mishra</p>
```

Add this line (example):

```html
<p><strong>Deployed by:</strong> DMI Cohort 2 | Rahul Sharma | Group 4 | Week 1 | 16-01-2026</p>
```

Footer Component

This project includes a responsive footer component that automatically displays the current year.
The goal is to avoid hard-coding dates so the footer stays accurate without manual updates.

What the footer does

Displays a copyright notice

Automatically updates the year based on the system date

Keeps the UI consistent across deployments

Dynamic Date Logic

The year is generated dynamically using JavaScript’s built-in Date object.
Each time the page loads, the current year is calculated and injected into the footer.

This ensures the footer always reflects the correct year without requiring code changes.

Code Snippet
<footer>
  <p>© <span id="year"></span> Pravin Mishra. All rights reserved.</p>
</footer>

<script>
  document.getElementById("year").textContent = new Date().getFullYear();
</script>


✅ This proof must be visible in your browser screenshot submission.