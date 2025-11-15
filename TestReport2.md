#  Website Test Report – CryptoGen Nepal

**Date:** 10/11/2025  
**Website URL:** [https://cryptogennepal.com](https://cryptogennepal.com)  
**Tested by:** Aryan Neupane  
**Test Date:** 10/11/2025  
**Test Report Submitted on:** 10/11/2025  
**Module:** Testing Website  
**Test Priority:** Medium  
**Test Type:** Functional + UI + Security  
**Submitted to:** Sandeep Chalise  

---

##  Pre-requirements

- Website accessible via [https://cryptogennepal.com](https://cryptogennepal.com)  
- Internet connection stable  

---

##  Platforms Tested On

- **Microsoft Edge (Windows 11)**  
- **Brave Browser (Windows 11)**  
- **Samsung Galaxy A25 (Mobile)**  

---

##  Detailed Test Cases

| **Test Case ID** | **Test Steps** | **Expected Result** | **Actual Result** | **Status** | **Comments** |
|------------------|----------------|----------------------|-------------------|-------------|---------------|
| **TC_001 – “Book Consultation” Button** | Click “Book Consultation” on homepage | Should open a working Calendly (or embedded form) page for scheduling. | Opens Calendly page showing “This Calendly URL is not valid.” | ❌ Fail | Broken external integration. Needs valid Calendly or internal booking form. |
| **TC_002 – Navigation Menu Check** | Click Home, About, Services, Resources, Contact | Each link should navigate smoothly to its section or page. | Navigation working but transitions slightly slow. | ⚠️ Partial Pass | Links functional, but transitions need optimization. |
| **TC_003 – Responsiveness** | Test site on mobile view | Layout should adjust to mobile screen without overlap. | Site generally responsive, but some text overlaps near hero image. | ⚠️ Partial | Needs minor CSS fixes for smaller devices. |

---

##  Post-Conditions

- “Book Consultation” link is **non-functional** (invalid Calendly integration).  
- Navigation is **partially functional**, but animations and transitions feel sluggish.  
- Mobile responsiveness is mostly fine but requires small CSS layout corrections.  
 

---

##  Recommendations

1. **Fix or replace the broken Calendly link** for the “Book Consultation” button.  
2. **Improve mobile responsiveness**, especially hero text alignment and padding.  
3. **Add an alternative booking form** (direct email or embedded form) in case Calendly fails.  
4. **Conduct a full mobile-device QA test** across various screen sizes (iOS and Android).  


---

**Prepared by:** Aryan Neupane  
**Submitted to:** Sandeep Chalise  
**Date:** 10/11/2025
