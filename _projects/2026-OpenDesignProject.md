---
layout: project
title: "Semester Design Project"
math: true
description: "MAE 2250 - Intro to Mechanical Design"
technologies: [LaTeX]
image: "/assets/images/brslogo.png"
fontsize: 11pt
geometry: margin=1in
papersize: letter
pagestyle: empty
header-includes:
- '\pagenumbering{gobble}'
- '\usepackage{url}'
- '\usepackage{enumitem}'
- '\usepackage{graphicx}'
- '\def\UrlBreaks{\do\/\do-\do\.\do\&\do\_\do?\do\#\do\=\do\%\do\~}'
- '\makeatletter'
- '\renewcommand{\section}{\@startsection{section}{1}{0pt}{2pt}{1pt}{\normalfont\Large\bfseries}}'
- '\renewcommand{\subsection}{\@startsection{subsection}{2}{0pt}{1.5pt}{0.5pt}{\normalfont\large\bfseries}}'
- '\makeatother'
---
## Table of Contents
- [Client Pitch](#client-pitch)
- [Functional Prototype](#functional-prototype)

# Client Pitch


**Team:** _Big Red Stompers_
**Clients:** Cornell CALS Extension / E\&J Gallo Winery / National Grape


## Problem Statement
Spotted lanternflies (SLF) mainly target grapevines. As a result, grape farmers are trying to manage SLF populations in vineyards and nearby trees. SLF egg masses contain around 30-60 eggs, creating rapid population growth that affects later growing seasons. Current SLF population reduction methods, such as netting and manual egg removal are difficult to scale across larger vineyards.


## Impact
Elimination of SLF eggs prevents the development of adult populations causing the most damage to vineyards. The average SLFs per vine starts low, increasing sharply following the transition from nymph to adult stages (Figure 1). As a result, attacking the root cause would protect regions like Lake Erie and the Finger Lakes from losses between $1.5 million in year one and $8.8 million by year three of infestation (Hayes).


## Proposed Concept: Stomp n' Scrape
**What it is:** Handheld egg removal device.


**How it would be used:** Designed to crush SLF egg mass shells and immediately scrape them into a rubbing-alcohol-filled vessel to prevent hatching.


**Why it’s better than the status quo:**


- Reduces the chance of leaving viable eggs behind.
- Minimizes mess and user discomfort by sealing egg material instantly.
- Improved output and efficiency compared to manual scraping alone.


**End-of-semester proof-of-concept:** A functional prototype with a crushing feature, integrated scraper, and removable alcohol container, fabricated using 3D-printed components and accessible materials, and tested on simulated SLF egg masses to evaluate effectiveness and ease of cleaning.


## Key Risks / Unknowns


- 1 - Egg masses harden, making it difficult to ensure they are fully damaged. Two methods to kill the egg masses: crushing them and then scraping them into rubbing alcohol to kill the remaining ones.
- 2 — Public aversion to kill/interact with SLF, as crushing egg masses may be off-putting. Test with user trials and gauge user comfort.
- 3 — Many eggs are laid on high surfaces; 98% of eggs are found at unreachable heights (+10 feet) on trees (Krawczyk). Test attachments to extendable tools for users to reach higher egg masses.


## Questions for Client
1. **What is preventing you from currently targeting egg masses? Is it location, time or resources?**
  *Decision affected:* This would affect the aspects we want to emphasize in our design, like making it accessible to higher areas of the tree and ease to clean, based on client demand.
2. **Are there methods for reaching high areas that you are currently using?**
  *Decision affected:* This would affect whether our product must account for reaching high-up areas, or if it can be used with existing tools.
3. **How much would you need to reduce or eliminate SLF after they’ve already reached the grapevines?**
  *Decision affected:* This would affect our focus from egg masses, potentially shifting our direction to solving the problem of SLFs in their adulthood phase.




## References

- New York State Integrated Pest Management. (n.d.). Spotted lanternfly management. https://cals.cornell.edu/integrated-pest-management/outreach-education/whats-bugging-you/spotted-lanternfly

- Hayes, C. (2025, January 27). Spotted lanternflies could cost NYS grape industry millions. Cornell Chronicle. https://news.cornell.edu/stories/2025/01/spotted-
    lanternflies-could-cost-nys-grape-industry-millions#:~:text=Using%20data%20from%20two%20key,and%20third%20years
    %20of%20infestation%2C.

- Krawczyk, G. (2023, August 30). What should you do with spotted lanternfly egg masses? PennState Extension. https://extension.psu.edu/what-should-you-do-with-spotted-lanternfly-egg-masses


## Figure


![Average SLFs per Vine (2018-2020)]({{ "/assets/images/avg_slf_per_vine.png" | relative_url }}){: style="max-width:100%; width:450px; height:auto; display:block; margin:0 auto;"}
---

---
# Functional Prototype

---

## In This Section
- [Design Intent and Functionality](#design-intent-and-functionality)
- [Parts List and Fabrication Details](#parts-list-and-fabrication-details)
- [Assembly Process](#assembly-process)
- [Design Tests](#design-tests)
- [Success Criteria](#success-criteria)
- [Exhibit-Day Demonstration Criterion](#exhibit-day-demonstration-criterion)

---

## Design Intent and Functionality

The prototype is intended to combine three main functions into one handheld device:

- **Scraping:** the scraper removes the spotted lanternfly egg mass off the surface.
- **Crushing / Stomping:** a spring-loaded internal stomper compresses the egg mass material to destroy the eggs.
- **Collection:** the lower opening funnels egg residue into an attached bottle for containment and later neutralization.

---

## Parts List and Fabrication Details

The functional prototype consists of the following parts:

| Part | Fabrication | Description |
|------|-------------|-------------|
| Housing | 3D printed at RPL | Contains the sliding rail, supports the scraper assembly, and connects to the bottle interface |
| Stomper Face | 3D printed at RPL | Translates along the internal rail and compresses the egg mass during actuation |
| Compression Spring | McMaster spring 8969T983 | Additional spring testing performed with a workshop spring better matched to intended hand-actuated displacement |
| Knob / Actuation Interface | 3D printed at RPL | Used by the user to pull the internal mechanism and compress the spring |
| Scraper | 3D printed at RPL | Removes egg masses from the surface and guides debris toward the bottle attachment |
| Bottle Thread Connector | 3D printed (lower housing) | Interfaces with a standard plastic bottle for residue collection |

---

## Assembly Process

1. **Prepare the spring-and-rod subassembly** — Place the compression spring onto the rigid rod. The front circular plate and the rigid rod are designed as a single 3D-printed part, so the spring is seated directly onto this rod-and-plate subassembly.

2. **Prepare the shell casing** — Take the printed shell / housing and inspect the rear opening to confirm that the spring-loaded subassembly can be inserted without interference.

3. **Insert the spring-loaded plate into the housing** — Slide the plate-with-spring subassembly into the shell casing through the rear opening so that the spring and rod align with the internal axis of the housing.

4. **Attach the pull knob** — Screw the pull knob onto the exposed end of the rigid rod at the back of the housing. This creates the user-actuated interface for compressing the spring.

5. **Install the scraper** — Thread the scraper through the back opening of the housing and position it so that it aligns with the front opening where the egg mass will be contacted.

6. **Attach the scraper plate to the rigid rod** — Secure the scraper plate to the rigid rod so that motion of the rod and spring mechanism drives the scraper/stomping action.

![Components and Functions Illustration](/assets/images/Components_and_Functions_Illustrations.png)
*Components and Functions Illustration*

---

## Design Tests

### Test 1: Sliding Rail Motion and Interference

**Part being tested:** Housing rail and slider/stomper interface.

**What is being tested:** Whether the slider can move through its intended range of motion without excessive friction, jamming, or interference. Because the product relies on repeated manual actuation, low-friction motion is critical for usability and repeatability.

**How it was tested:** The force required to initiate motion was measured using a spring-force ruler / spring scale attached to the slider. In addition, all 5 team members operated the slider and rated ease of use on a scale from 1 to 10, where 1 indicates very easy operation and 10 indicates very difficult operation.

**Results:** During assembly and initial actuation, the rail exhibited excessive friction due to insufficient CAD tolerance and printing inaccuracy. The force required to initiate motion was 10 N. The mean user difficulty score before modification was 7/10, indicating poor usability. After sanding the rail surfaces, the slider moved more smoothly and the mean user difficulty score improved to 5/10, but this remained outside the desired usability range of 1–4.

**Conclusion / design changes for next prototype:** The next prototype will increase clearance tolerances between the housing and slider by 5 mm and switch from PLA to PETG to reduce print irregularities and improve sliding performance. Additional testing over repeated cycles will be conducted to confirm that the rail does not bind over time.

---

### Test 2: Spring Mechanism Force and Usability

**Part being tested:** Compression spring and stomping mechanism.

**What is being tested:** Whether the spring can be compressed by hand while still supplying enough force to help crush the egg mass. The design target from earlier work was a force in the approximate 50–70 N range, and the spring constant needed to be appropriate for the intended user displacement.

**How it was tested:** The team first evaluated the McMaster spring by manually compressing it through the intended actuation path and observing whether a user could reasonably generate sufficient displacement. The team then tested a workshop spring and estimated its spring constant using Hooke's Law from an applied 500 g load and the resulting displacement of 1.5 in.

**Results:** The McMaster spring was too stiff for practical hand use and could only be compressed by several millimeters, which was far below the required displacement. A replacement spring from the workshop displaced 1.5 in under a 500 g force, corresponding to a spring constant of approximately 129 N/m or 0.74 lb/in. This value was close to the team's rough estimated range, but later trials suggested that to more confidently generate sufficient crushing force with a displacement of about 2 in (~50 mm), the design would require a higher spring constant of approximately 3–3.5 lbf/in.

**Conclusion / design changes for next prototype:** The next prototype will use a spring with a slightly higher spring constant than the workshop spring while still remaining hand-operable. The team will also redesign the rod/attachment geometry to improve load transfer between the spring and stomper.

---

## Success Criteria

Our project aims to create a portable product that provides a faster, cleaner, and more effective way to destroy spotted lanternfly egg masses than current scraping methods. For the final prototype, success will be evaluated using the following quantitative criteria.

### Criterion 1: Portability
The device must weigh no more than **0.5 kg** and have a length no greater than **20 cm** without the bottle attachment and **30 cm** with the bottle attachment. This criterion assesses portability and ease of handling. It will be measured using a digital scale and ruler. Smaller values are beneficial but are not the highest priority.

### Criterion 2: Egg Destruction Effectiveness
The device must destroy at least **95%** of the eggs in one egg mass in a single use. This criterion assesses the effectiveness of the crushing mechanism. It will be measured using a substitute egg mass such as peas and/or Orbeez, with the number of intact versus destroyed units counted before and after one actuation. A higher percentage is a high priority.

### Criterion 3: Removal Speed
One egg mass must be completely removed and destroyed in less than **10 seconds** on average. This criterion assesses efficiency in realistic use. It will be measured with a stopwatch across 10 repeated trials, using the average completion time. Faster completion is a very high priority.

### Criterion 4: Residue Capture
The device must funnel at least **80%** of the egg residue into the attached bottle. This criterion assesses cleanliness and collection performance. It will be measured by comparing the mass or count of collected residue in the bottle to the total removed residue. Increasing the capture percentage is a high priority.

### Exhibit-Day Demonstration Criterion

Our exhibit-day demonstration will focus on two criteria that produce visible and measurable outcomes: complete egg-mass removal in under 10 seconds and at least 80% residue capture in the bottle. During the demo, the team will use a substitute egg mass on a test surface, time the removal process, and show that most of the residue is visibly directed into the bottle attachment.