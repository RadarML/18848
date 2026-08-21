---
hide:
- navigation
---

# 18-848 **Machine Learning for Radar**

Radio Frequency (RF) sensing is a critical component of modern autonomous systems. For example, mmWave radars are ubiquitous in modern vehicles and a key part of autonomous driving systems. Due to their robustness, compact form factor, low cost, and privacy-preserving nature, RF sensing systems are also increasingly used for many indoor and human sensing applications.

To unlock the full potential of these sensors, we naturally turn to machine learning (ML), which has revolutionized how we approach sensing and perception, particularly in the computer vision community. However, to date, there has been relatively little overlap between the RF and ML communities, with relatively limited work on sensing methodologies which integrate RF and machine learning at a more fundamental level. Modern machine learning paradigms such as large-scale foundation models have also yet to be fully explored for the RF domain.

!!! warning "Registration / Waitlist"

    While 18-848 currently shows as waitlisted due to seat reservations for specific programs, the course is not actually full.
    
    **If you are waitlisted, you should be added to the course within the first 1-2 weeks**. Please come to class and participate regardless!


<div class="grid cards speakers">

<div class="card speaker">
    <img class="speaker-photo" src="people/tianshu.jpg" alt="Tianshu Huang">
    <div class="speaker-body">
        <div class="speaker-name">
            Instructor: Tianshu Huang
        </div>
        <div class="speaker-topic">tianshu2@andrew.cmu.edu</div>
        <div class="speaker-title">Office Hours: TBD or by appointment</div>
    </div>
</div>

<div class="card">
    <div class="speaker-body">
        <div class="speaker-name">Lecture: Tuesday / Thursday, 12:20–1:50pm</div>
        <div class="speaker-title">Porter Hall 125B</div>
    </div>
</div>
</div>

## Overview

This research-focused course will provide students with ML **and/or** RF background the knowledge and skills needed to effectively engage in cross-disciplinary collaborations which push the frontiers of Machine Learning for RF.

The course will feature traditional lectures covering key background, such as the fundamentals of modern FMCW radars and machine learning research methodologies for scaling up ML research for novel domains, as well as research lectures covering the current state-of-the art and guest lectures from academic researchers and industry insiders. Students will also gain hands-on experience working with wireless systems such as mmWave radars and spectrum analyzers, as well as large datasets collected from these systems to develop, train, and apply modern machine learning techniques such as self-supervised learning and scaled-up transformer models. Finally, students will complete a research project applying Machine Learning techniques to mmWave radar or an RF system of their choice.

### Prerequisites

This course is intended for graduate students and advanced undergraduate students. All students are expected to have some machine learning background (e.g., 10-202, 10-301, or 18-661), be familiar with programming in Python (e.g., to use ML frameworks such as Pytorch), and have at least undergraduate-level linear algebra and probability background.

In addition, students should either have further machine learning or wireless communications background:

<div class="grid cards" markdown>

- **Machine Learning**

    Any upper-division or graduate-level ML course, e.g., any 10-6XX or 10-7XX course.

- **Wireless Systems**

    Any wireless communications course, e.g., 18-750 or 18-452.

</div>

### Assignments and Grading

Grading will be based on the following assignments:

**Lab assignments (30%)**: students will individually complete the following labs:

- Radar systems (15%): configuring, collecting, processing, and visualizing data from a mmWave radar (AWR1843AOPEVM).
- Machine learning on radar data (15%): training a radar model and running ablations.

**Course project (50%)**: students will complete a course project in groups of up to 4 students (students may form groups of any size, including individually). Students are encouraged to form groups with complementary skill sets and to select projects which are aligned with other concurrent research activities if applicable.

Each project must involve some form of machine learning training and/or inference, and must involve some form of radar or other RF hardware, either for data collection and/or online deployment.

The project will be split into the following milestones:

- Project proposal (10%)
- Midterm progress report (10%)
- Final presentation (10%)
- Final report (20%)

**Presentation and paper review (15%)**: students will present a paper of their choice from the radar, ML, and related literature as part of student-led discussions.

**Class participation (5%)**: As a research-focused course, we understand that students often have conflicting commitments (e.g., conferences). We expect students to attend and actively participate whenever possible, and notify the instructors in advance if they will be unable to attend class. We may also ask students to make specific preparations (e.g., discussion questions) in advance of guest lectures.

## Topics

This class is not a conventional lecture-based course, and will be roughly split into three components:

1. **Introductory Lectures**: lectures covering the fundamentals of radar and machine learning with a focus on understanding key concepts, tradeoffs, and considerations.

    Crucially, our goal is to provide enough high-level understanding that students can effectively collaborate with experts in complementary domains. As such, while the radar and machine learning portions are primarily targeted at students with limited background in these respective areas, we aim to provide an orthogonal, high-level perspective which students with more experience will also find useful.

2. **Student-led Seminars**: students will lead discussions on papers of their choice covering the state of the art in domains such as wireless sensing, foundation models, computational imaging, simulation, and other areas of interest.

    Students are encouraged to select papers which are aligned with their technical background and interests.

3. **Guest Lectures**: this course will feature a substantial number of guest lectures with speakers from both academia and industry, covering a wide range of topics related to radar and machine learning.

### Guest Speakers

::: speakers

## Schedule

!!! warning "Subject to change"

    The course schedule is subject to change, particularly with regards to the timing of guest lectures.
    
    Updates will be announced in class; you can also check here for changes.

::: schedule
