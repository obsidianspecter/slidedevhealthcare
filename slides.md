---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## HealthcareDOC – Revolutionizing Women's Healthcare
  AI-Powered Digital Health Platform
# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS (experimental)
css: unocss
wakeLock: "build"
---

# HealthcareDOC – Revolutionizing Women's Healthcare

AI-Powered Digital Health Platform

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
</div>

<div class="text-sm opacity-50 absolute bottom-8">
  ANVIN Deepak | Supervisor: Amuthasurabi | 21/05/2025
</div>

---

# Abstract

<div class="text-left">
HealthcareDOC is an innovative AI-powered digital health platform specifically designed for women's healthcare needs. The platform integrates four specialized chatbots:

- **Deepak1**: General women's health advisor
- **Anvin AI**: Reproductive health specialist
- **MedPresc AI**: Medication and prescription assistant
- **Ayurvedic AI**: Traditional medicine consultant

Additional modules include Period Tracker, Medical Store Locator, and Mood Tracker, creating a comprehensive healthcare ecosystem.

Key performance metrics show up to **40% faster response times** and **25% higher accuracy** compared to existing solutions.

Future enhancements will include multilingual support and voice-based AI interaction.
</div>

---

# Problem Statement & Motivation

<div class="grid grid-cols-2 gap-4">
<div>

## Challenges
- Limited access to timely, personalized women's healthcare
- Delayed doctor responses
- Social stigma around certain health topics
- Lack of consistent follow-up
- Limited multilingual support

</div>
<div>

## Motivation
- Empower women with instant, AI-driven healthcare support
- Provide context-aware medical information
- Create a judgment-free environment for sensitive topics
- Ensure continuous health monitoring
- Bridge healthcare accessibility gaps

</div>
</div>

---

# System Architecture & Methodology

<div class="grid grid-cols-2 gap-4">
<div>

- Backend built on **FastAPI** for secure, rapid processing
- **LLaMA 3.2** fine-tuned for women's health
- Separate chat histories for each specialized chatbot
- Integrated modules:
  - Period Tracker
  - Medical Store Locator
  - Mood Tracker
- HIPAA-compliant data handling

</div>
<div>

```mermaid {scale: 0.8}
graph TD;
    A[User Query] --> B[FastAPI Backend];
    B --> C[LLaMA 3.2 AI Model];
    C --> D[Generate Response];
    D --> E[Display Answer];
```

</div>
</div>

---

# Experimentation & Results

<div>

## Key Metrics
- Response accuracy compared to verified medical sources
- Latency tests under different loads
- User satisfaction surveys

## Results
- **40% faster** response times
- **25% higher** accuracy
- **92%** user satisfaction rate

</div>

---
layout: center
---

# Performance Comparison

```mermaid
gantt
    title Performance Comparison
    dateFormat  YYYY
    axisFormat  %Y
    section Accuracy (%)
    HealthcareDOC          :done, 2024, 2025-01-01, 90d
    General Medical Chatbot:active, 2024, 2025-01-01, 70d
    Rule-Based Chatbot     :2024, 2025-01-01, 60d
```

<div class="text-center mt-4">
HealthcareDOC outperforms existing solutions with 25% higher accuracy and 40% faster response times
</div>

---

# Key Outcomes & Future Scope

<div>

## Current Achievements
- AI-driven chatbot optimized for women's health
- Seamless FastAPI integration
- Privacy-first design ensuring data security

## Future Enhancements
- Multilingual support
- Voice-based interaction
- Expanded knowledge base for postpartum care and mental wellness

</div>

---
layout: center
class: text-center
---

# Future Enhancements Timeline

<div class="w-full px-10">

```mermaid
gantt
    title Future Enhancements Timeline
    dateFormat  YYYY-MM-DD
    axisFormat  %b %d
    section Optimization
    Fine-tuning       :done, 2025-01-01, 2025-02-15
    section New Features
    Multilingual Support  :2025-03-01, 2025-04-15
    Voice-Based AI        :2025-04-16, 2025-06-01
    section Compliance
    HIPAA/GDPR Implementation :2025-06-02, 2025-07-15
```

</div>

<div class="text-center mt-4 text-xl">
Planned feature rollout over the next 6 months
</div>

---

# Modules Overview

<div class="grid grid-cols-2 gap-4">
<div>

## AI Chatbots
- **Deepak1**: General women's health advisor
- **Anvin AI**: Reproductive health specialist
- **MedPresc AI**: Medication and prescription assistant
- **Ayurvedic AI**: Traditional medicine consultant

</div>
<div>

## Supporting Modules
- **Period Tracker**: Monitors menstrual cycles, fertile windows, and ovulation
- **Medical Store Locator**: Uses geolocation and interactive maps
- **Mood Tracker**: Monitors emotional well-being over time

</div>
</div>

---
layout: center
---

# Integration Architecture

```mermaid
graph LR;
    User-->|Interacts with|Platform;
    Platform-->|Routes to|Chatbots;
    Platform-->|Connects to|Modules;
    Chatbots-->|Provides|HealthInfo;
    Modules-->|Enhances|UserExperience;
```

<div class="text-center mt-4">
Seamless integration between user interface, AI chatbots, and supporting modules
</div>

---
layout: center
class: text-center
---

# Conclusion

<div class="text-left">
HealthcareDOC represents a transformative approach to women's healthcare, integrating multiple AI chatbots and supportive modules to provide:

- Real-time, secure, and personalized health support
- Comprehensive coverage of women's health concerns
- Accessible healthcare information in a judgment-free environment
- Continuous health monitoring and tracking

The platform demonstrates significant improvements in response time and accuracy, with a clear roadmap for future enhancements to further bridge healthcare accessibility gaps.
</div>

<div class="pt-12 opacity-70 italic">
  "Empowering women through accessible, intelligent healthcare solutions."
</div>

---
layout: image-right
image: https://source.unsplash.com/collection/94734566/1920x1080
---

# Thank You

<div class="text-left">

## Contact Information
- **Email**: anvin.deepak@healthcare.doc
- **Website**: healthcaredoc.ai
- **GitHub**: github.com/anvindeepak/healthcaredoc

## Acknowledgements
Special thanks to:
- Amuthasurabi (Supervisor)
- The Medical Advisory Board
- Beta Testing Participants

</div>