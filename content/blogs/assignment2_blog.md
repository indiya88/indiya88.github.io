---
date: '2026-02-19T12:54:29-05:00'
draft: true
title: 'Survey Secrets'
tags: ["data-ethics","survey design"]
categories: ["blog"]
---
## When ‘Anonymous’ Data Isn’t Really Anonymous

Hey friends!

Data science is amazing! We get to uncover insights, help organizations improve, and even make life a little easier for people. But with great data power comes great ethical responsibility. As Luciano Floridi explains in Chapter 4 of *The Ethics of Artificial Intelligence*, AI represents a new form of agency that brings serious ethical challenges. (Floridi, 2023, p. 57).

I’ve been exploring the ethical side of data science, and I realized that even something as simple as a post-course survey can hide tricky ethical dilemmas.

---

### The Scenario: A Course Feedback Survey

Imagine you’ve been asked to analyze a post-course survey. Participants complete a 10-question survey after finishing their course.

**The survey:**

- Requires participants to log in with organizational credentials.
- Claims all responses will remain anonymous.
- Asks for the course name but not the participant’s personal name.

Executive management wants you, the data analyst, to provide actionable insights on which courses might need redesigning.

---

Here’s what the first survey question looks like:

> “This course met all of the course objectives.”  
> *(0–10 scale from Strongly Disagree → Strongly Agree)*

---

## 1) Ethical Issues in Survey Design and the Sample Question

Even this single question raises several ethical red flags:

### Anonymity vs. Login Requirement

The survey says responses are anonymous… but it also requires students to log in with their organizational accounts and that feels contradictory. If participants believe their answers can’t be traced back to them, but technically the system could connect responses to their login credentials, it creates a problem with **autonomy**.

Autonomy means respecting individuals’ ability to make informed decisions about their own data. People can’t fully control their data if they don’t clearly understand how it’s being handled. It also raises concerns about **explicability**, which Floridi defines as ensuring both intelligibility “how does it work?” and accountability “who is responsible?”   (Floridi, 2023, p. 63).

Lack of clarity here can diminish trust with students, which may reduce participation or honesty.

---

### Course Name Collection

The survey asks for the course name but not the participant’s name. At first, this seems anonymous… but if a course only has eight students, it could be easy to identify someone.

This raises **nonmaleficence** concerns, the principle of avoiding harm (Floridi, 2023, p. 61). Even unintentional disclosure could cause harm. Privacy protection isn’t just about removing names; it’s about anticipating indirect ways participants could be identified.

---

### Ambiguity in Survey Questions

The sample question, *“This course met all of the course objectives,”* is vague. What exactly does “met all objectives” mean? Practical skills? Theory? Enjoyment?

Different interpretations lead to inconsistent responses, affecting **justice**, which requires fairness in how systems impact individuals and groups (Floridi, 2023, p. 62). Courses could be redesigned based on unreliable feedback, unfairly affecting instructors or students.

On top of that, the interface itself introduces errors. Participants select a number on a 0–10 scale, but as you scroll, some options disappear, making it easy to accidentally choose the wrong number. This reduces **explicability** (Floridi, 2023, p. 63) because participants can’t clearly understand or respond accurately, which ultimately compromises fairness and reliability.

---

### Real-World Example

I’ve personally seen survey issues in class before. One class required us to complete a survey to access assignment submissions. It felt forced and not truly voluntary. This shows how survey design can compromise **autonomy** (Floridi, 2023, p. 61). Students might give rushed or dishonest answers, and the data collected may not reflect genuine feedback.

---

## 2) Other Ethical Issues That Could Be Present

Beyond the obvious concerns, several additional ethical issues could arise:

 - **Voluntariness:** If students feel pressured to participate, responses may not be honest, affecting **beneficence**, which promotes well-being and positive outcomes (Floridi, 2023, p. 60).
- **Data Storage and Access:** Lack of transparency risks privacy violations.
- **Bias in Interpretation:** Poor interpretation might lead to unfair decisions, violating **justice** (Floridi, 2023, p. 62).
- **Security Risks:** Weak security could cause harm, raising **nonmaleficence** concerns (Floridi, 2023, p. 61).
- **Transparency to Participants:** Without clarity, the survey lacks **explicability** (Floridi, 2023, p. 63).

---

## 3) Recommendations for Executive Management

Here’s how to address these issues while still producing actionable insights:

- Clarify anonymity and separate login credentials from survey data.
- Be transparent about how data is stored and used.
- Make participation optional.
- Audit survey questions for clarity and neutrality.
- Encrypt responses and restrict access.
- Analyze responses in aggregate to promote fairness and justice (Floridi, 2023, p. 62).

---

## 5 Key Ethics Concepts Applied

The ethical concerns in this survey directly reflect the unified framework described in Chapter 4 of *The Ethics of Artificial Intelligence* (Floridi, 2023, pp. 60–63):

1. **Autonomy** – ensuring participants control their personal data.
2. **Beneficence** – using data to benefit participants and society.
3. **Nonmaleficence** – avoiding harm, such as privacy breaches.
4. **Justice** – ensuring fairness in interpretation and decision-making.
5. **Explicability** – making data systems transparent and accountable.

These concepts are practical guides for survey design, data collection, and reporting.

---

## 4) Proceeding Ethically if Recommendations Are Rejected
      
If executive management rejects ethical recommendations, a data analyst still has professional responsibilities. One ethical step is to document concerns clearly, ensuring transparency about potential risks or limitations in the survey design. The analyst can also reduce harm through responsible reporting by including context about bias, privacy concerns, or data quality when presenting results. This supports justice and nonmaleficence by preventing unfair or misleading conclusions (Floridi, 2023, pp. 61–62).
       
If needed, concerns can be raised through appropriate professional channels, such as a supervisor or data governance process, while maintaining respect and professionalism. Even wherecommendations are declined, analysts can uphold ethical standards by communicating findings honestly and encouraging transparency in how the data is used.

---

## Conclusion: Ethics is Everyone’s Business

Even a simple survey can hide a world of ethical challenges. By considering autonomy, beneficence, nonmaleficence, justice, and explicability, we protect participants, improve trust, and produce more reliable, actionable insights.

Data science isn’t just about numbers — it’s about people. Ethical principles help us make data work for everyone, not just for organizational efficiency.

So next time you log in to a survey, remember: the ethical choices behind the scenes are just as important as the insights that come out.

---

## References

Floridi, L. (2023). *The Ethics of Artificial Intelligence*. Oxford University Press.
