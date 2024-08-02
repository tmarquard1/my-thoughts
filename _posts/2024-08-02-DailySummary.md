---
title: "Random Daily Debrief"
date: 2024-08-02
---

**Side note**: Why doesn't everyone format YYYY-MM-dd? It just makes so much more sense.

### Debrief - August 2, 2024

**Insights:**

1. **MTU Issues with Pip Installs in Docker:**
   - **Problem:** Pip installs can fail in a Docker container due to MTU (Maximum Transmission Unit) discrepancies.
   - **Cause:** Host network discovery level MTU and default MTU in Docker might not always match.
   - **Environment:** 
     - Mac M1 Max
     - 64 GB RAM
     - macOS Version 14.5
     - Docker v4.33.0
   - **Solution:** Updated Docker daemon setting to set the MTU to 1400. [Stack Overflow Reference](https://stackoverflow.com/questions/50846943/using-pip-in-docker-container-leads-to-readtimeouterror)

2. **AWS Permission Boundary:**
   - **Meeting Attendees:** Carter, Scott K, Howard, and Talon Marquard
   - **Problem:** Need to add a Permission Boundary to the CDK bootstrap of AWS accounts to prevent account escalation in case of permission leaks.
   - **Action Items:**
     - **Carter:** Start working on the permission boundary policy document.
     - **Howard:** Work on adding and updating the permission boundary policy on AWS accounts.

3. **Meeting with Aaron:**
   - **Main Focus:** Aaron learning more about the applications.
   - **Plan:**
     - Aaron could help Lisa Marie as the product owner to understand the application from the customer's perspective.
     - Aaron is good at documenting, and Talon is good at explaining things.
     - They will work together three times a week for a short duration to update nView documentation.