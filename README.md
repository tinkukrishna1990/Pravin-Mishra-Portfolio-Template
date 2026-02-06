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

Footer Requirement Readme:

1. Requirement to have dynamic date in the format for DD Mon YYYY. It's required to implement a script Js to call in the html using span tag.
2. Script how it's used.

<div class="footer-bottom">
		<p>Pravin Mishra Portfolio v1.0 - Deployed on <span id="deployDate"></span> - By <span>MOHANA KRISHNA DHARANI KUMAR</span></p>
      </div>

<script>
    //document.getElementById("deployDate").textContent = new Date().toLocaleDateString('default'); //it'll print in DD/MM/YYYY
	
	document.getElementById("deployDate").textContent =
		new Date().toLocaleDateString("en-GB", {
		 day: "2-digit",
		 month: "short",
         year: "numeric"
    });

  </script>
  


✅ This proof must be visible in your browser screenshot submission.