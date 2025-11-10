# 🧾 Website Test Report – Butwal Multiple Campus

**Date:** 06/11/2025  
**Website URL:** [http://bumc.edu.np](http://bumc.edu.np)  
**Tested by:** Aryan Neupane  
**Test Date:** 06/11/2025  
**Test Report Submitted on:** 06/11/2025  
**Module:** Testing Website  
**Test Priority:** Medium  
**Test Type:** Functional + UI + Security  
**Submitted to:** Sandeep Chalise  

---

## 🧩 Pre-requirements

- Website accessible via [https://bumc.edu.np](https://bumc.edu.np)  
- Internet connection stable  
- Cache cleared before testing  

---

## 💻 Platforms Tested On

- **Microsoft Edge (Windows 11)**  
- **Brave Browser (Windows 11)**  
- **Samsung Galaxy A25 (Mobile)**  

---

## 🧪 Detailed Test Cases

| **Test Case ID** | **Test Steps** | **Expected Result** | **Actual Result** | **Status** | **Comments** |
|------------------|----------------|----------------------|-------------------|-------------|---------------|
| **TC_001 – SSL Certificate Validation** | Open [https://bumc.edu.np](https://bumc.edu.np) | Site should use secure HTTPS connection and show a valid SSL certificate. | Browser shows **“Not Secure”** warning — certificate missing or expired. | ❌ Fail | Major security issue; SSL must be configured. |
| **TC_002 – Testimonial Section** | Scroll to *“Voice from Our Students”* | Should display real testimonials with name, image, and feedback. | Shows placeholder *Lorem ipsum* text and only one student entry. | ❌ Fail | Needs real data and multiple working slides. |
| **TC_003 – Downloads Section** | Click “Registration Form” & “Admission Form” | Download should start or open the file in browser. | Links visible but no files downloaded (unresponsive). | ❌ Fail | File URLs may be broken or missing. |
| **TC_004 – Navigation Buttons** | Test “Home”, “About Us”, “Programs”, “Research Cell”, “Notices” | Each button should redirect to relevant working page. | Navigation menu loads, but some links return blank/slow loading pages. | ⚠️ Partial Fail | Optimize links and page routing. |
| **TC_005 – Loading Performance** | Manual page load observation | Should load within **3 seconds** on stable connection. | Takes **6–8 seconds** to load hero and main content fully. | ⚠️ Partial Fail | Optimize images and remove unnecessary scripts. |
| **TC_006 – Footer Links** | Scroll down to footer | Footer links should redirect correctly and display copyright. | Footer present but links incomplete (“Quick Links” blank). | ❌ Fail | Missing important links and social media icons. |

---

## ✅ Post-Conditions

- User experience is **inconsistent** due to broken links, missing SSL, and incomplete UI sections.  
- Navigation is **partially functional**, but some forms and buttons need debugging and working file links.  
- Website lacks proper finishing and professional polish required for a public institutional site.  

---

## 🛠️ Recommendations

1. **Install a valid SSL certificate** (via *Let’s Encrypt* or *Cloudflare*) to secure the site.  
2. **Replace placeholder content** (“Lorem ipsum”) with real testimonials and text.  
3. **Fix broken “Download” links** for the Registration and Admission forms.  
4. **Improve navigation routing** — ensure all menu buttons open valid and active pages.  
5. **Optimize page loading speed** by compressing images and removing unused scripts.  
6. **Complete footer links** — include Quick Links, contact info, and social media icons.  
7. **Perform a responsive design check** on all devices (desktop, tablet, mobile).  
8. **Regularly audit website content** to maintain consistency, accessibility, and reliability.  

---

**Prepared by:** Aryan Neupane  
**Submitted to:** Sandeep Chalise  
**Date:** 06/11/2025
