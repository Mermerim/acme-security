## 📋 Submission Information

**Name:** [Mehmet Mermer]  
**Email:** [fmermerim@gmail.com]  
**LinkedIn:** [www.linkedin.com/in/mermerim](www.linkedin.com/in/mermerim)  
**Submission Date:** [2025-11-10]

---

## ✅ Deliverables Checklist

Please confirm you've included all required items:

- [x] **Report** (PDF, max 5 pages)
  - [x] Section 1: Incident Analysis
  - [x] Section 2: Architecture Review
  - [x] Section 3: Response & Remediation
  
- [x] **Video Presentation** (10-15 minutes)
  - [x] Link provided in `video_link.md`
  - [x] Video is accessible (tested in incognito)
  - [x] Duration is within guidelines

- [✅] **File Structure**
```
  submissions/firstname-lastname/
  ├── report.pdf
  ├── video_link.md
  └── notes.md (optional)
```

---

## 📊 Self-Assessment

**Time spent on this lab:** Approximately 7 hours

**Tools used:**
- Log analysis: Visual Studio - Rainbow Csv Plugin
- Diagrams: Canva
- Video recording: Obs Studio

**Confidence level:**
- [x] Very confident in my analysis
- [ ] Confident but some uncertainties
- [ ] Attempted my best with available knowledge

---

## 🎯 Brief Summary (2-3 sentences)

_Briefly describe your approach and key findings:_

By reviewing the necessary documentation, architecture, known vulnerabilities, planned penetration testing activities that could be considered "false positive," and log sources, I identified the attacker's IP address, 203.0.113.45. This resulted in a complete attack timeline, API BAC -> Phishing -> SQLi.

---

## 🔍 Key Findings Highlight

**Main attack vectors identified:**
1. API - Broken Object Level Authorization (BOLA)
2. Phishing Attack
3. SQL Injection - WAF Bypass and Data Exfiltration

**Most critical vulnerability:**

Data leakage resulting from SQL Injection has caused widespread damage.

**Top recommendation:**

Instead of "Basic Rules", "Managed Rule Sets" should be activated. These advanced rules are specifically designed to recognize and block known WAF circumvention, obfuscation and injection techniques such as /*!...*/. This way, even if the payload passes the "Basic Rules" filter, it will be stopped at this advanced layer.


---

## 💭 Challenges & Learnings

**What was most challenging?**
It took me a while to realize that the attacker was actually a penetration tester, and the chronological order of his attacks confused me at first.

**What did you learn?**
I did not expect to encounter the IDOR vulnerability in the broken access control attack.

**What would you do differently?**
I would run the penetration test ahead of time to create confusion.

---

## 📝 Additional Notes _(optional)_

Any context, assumptions, or additional information you'd like evaluators to know:

[Write here]

---

## ⚖️ Declaration

I declare that:
- [x] This work is entirely my own
- [x] I have not copied from other submissions or answer keys
- [x] I have not modified the provided log files
- [x] All sources and tools are properly attributed
- [x] I understand plagiarism results in disqualification

**Signature:** [Mehmet MERMER]  
**Date:** [2025-11-10]

---

## 🚀 Ready for Review

By submitting this PR, I confirm that my work is complete and ready for evaluation.

---

_Thank you for your submission! Our team will review it within 1 week._