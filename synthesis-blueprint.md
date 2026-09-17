# Assignment 02: Synthesis Blueprint

## DFIR First Steps: A Beginner's Investigation Roadmap

[← Professional Portfolio](https://lorenzojvillalobos.github.io/professional-portfolio/)  
[← DFIR Field Guide](https://lorenzojvillalobos.github.io/dfir-field-guide/)

---

## Project Overview

This synthesis project builds on my [DFIR Field Guide](https://lorenzojvillalobos.github.io/dfir-field-guide/) by transforming the resources I collected during Project 01 into a practical investigation roadmap for people entering Digital Forensics and Incident Response.

Project 01 focused on finding, evaluating, and organizing useful DFIR resources. For Project 02, I want to take the next step and show how those resources fit together during an actual investigation.

Instead of presenting another collection of tools and references, this project will explain how a cybersecurity incident moves from initial response through evidence preservation, examination, analysis, and continued training.

---

## 1. Audience Profile

My target audience is students, career changers, and entry-level cybersecurity professionals who are interested in Digital Forensics and Incident Response but do not yet have formal experience conducting an investigation.

The audience may already understand basic computer systems, networking, cybersecurity terminology, or operating systems. They may also have experimented with cybersecurity labs or tools. However, I do not assume that they already understand how a DFIR investigation is structured or how individual forensic tools fit into the larger investigative process.

One of the problems I found while building my Project 01 collection is that there is a large amount of DFIR information available, but it can be difficult for someone new to the field to understand where everything fits. A beginner may find tools such as Autopsy, Volatility, KAPE, or Wireshark without understanding when an investigator would use them, what type of evidence they examine, or how the results contribute to an investigation.

My goal is to fill that gap by creating a practical roadmap of the investigative process. The product will explain how an incident progresses from initial response through evidence preservation, examination, analysis, and reporting.

The guide is intended to be useful both as an introduction and as a reference. Someone learning DFIR could read it from beginning to end to understand the overall process, then return to individual sections later while completing labs, studying forensic tools, or practicing investigations.

---

## 2. Format Choice

I am creating a **beginner-focused DFIR investigation primer and reference guide** organized around the major stages of a digital investigation.

I chose this format because my intended audience does not need another list of cybersecurity tools or links. They need to understand how the pieces connect.

Organizing the information around the investigative process will allow readers to see what should happen first, why evidence must be preserved, what types of tools may be appropriate during different stages, how investigators interpret their findings, and how those findings eventually become investigative conclusions.

---

## 3. Annotated Outline

### 1. Recognizing an Incident and Starting the Investigation

This section will introduce what happens when suspicious activity is first discovered. It will explain why investigators must determine the scope of the incident, document their actions, establish responsibilities, and begin the response process without unnecessarily changing or destroying potential evidence.

The goal of this section is to show that an investigation begins before forensic software is ever opened. Decisions made during the first stages of an incident can affect the evidence available later.

**Sources:**

- NIST SP 800-61 Rev. 3 – *Incident Response Recommendations and Considerations for Cybersecurity Risk Management*
- CISA – *Federal Government Cybersecurity Incident and Vulnerability Response Playbooks*

---

### 2. Protecting and Preserving Digital Evidence

Before evidence can be analyzed, it must be collected and preserved correctly. This section will introduce evidence integrity, documentation, forensic acquisition, and the importance of avoiding unnecessary changes to original evidence.

It will also explain why evidence handling is part of the investigation itself rather than simply preparation for analysis. If investigators cannot demonstrate that evidence was collected and handled correctly, the reliability of their later findings can be questioned.

**Sources:**

- NIST SP 800-86 – *Guide to Integrating Forensic Techniques into Incident Response*
- SWGDE – *Best Practices for Computer Forensic Acquisition*

---

### 3. Beginning Endpoint Triage

This section will explain what investigators may examine first on an affected computer and how forensic triage can help determine where deeper analysis is needed.

It will introduce common Windows forensic artifacts such as Prefetch, LNK files, USB device history, UserAssist, and other evidence of user or system activity. It will also introduce tools such as KAPE that can quickly collect important forensic artifacts when investigators need information without immediately performing a complete forensic examination of a system.

The goal is to help beginners understand that investigators do not always begin by examining every file on a computer. Triage helps identify the evidence that deserves the most attention.

**Sources:**

- 13Cubed – *Introduction to Windows Forensics*
- KAPE – *Kroll Artifact Parser and Extractor*

---

### 4. Examining and Connecting the Evidence

Once evidence has been preserved and collected, investigators need to determine what actually happened. This section will explain how different evidence sources can provide different pieces of the same investigation.

Disk and file-system analysis can reveal stored files, deleted information, user activity, and system artifacts. Memory analysis can reveal running processes, network connections, loaded modules, and information that may only have existed while the computer was operating.

Network evidence can provide another perspective by showing communication between systems, protocols being used, and possible suspicious connections.

The purpose of this section is to show that investigators rarely rely on a single artifact. Conclusions are usually developed by connecting evidence from multiple sources.

**Sources:**

- Autopsy – *Digital Forensics Platform*
- Volatility 3 – *Volatile Memory Analysis Framework*

---

### 5. Connecting Evidence to Attacker Behavior

Finding an unusual file, process, or network connection is only part of an investigation. Investigators must determine what those findings mean and how they relate to the activity that occurred.

This section will introduce MITRE ATT&CK as a way to describe known attacker tactics and techniques. It will demonstrate how evidence discovered during an investigation can be connected to patterns of adversary behavior.

Sigma will also be introduced as an example of how attacker behavior can be translated into detection logic that may help identify similar activity in security logs.

This section will help move the reader from simply finding artifacts toward interpreting what those artifacts may reveal about an incident.

**Sources:**

- MITRE – *Getting Started with ATT&CK*
- Sigma – *Generic Detection Rule Format*

---

### 6. Building Investigation Skills Through Practice

The final section will focus on moving from understanding the investigative process to actually performing investigations.

DFIR is a field where reading about tools and procedures is not enough. Investigators need experience working with forensic images, packet captures, system artifacts, logs, and other forms of evidence.

This section will recommend beginning with controlled forensic datasets and then progressing into more realistic investigation scenarios. Resources such as the NIST CFReDS Hacking Case and CyberDefenders allow learners to practice examining evidence, answering investigative questions, and developing conclusions.

The goal is to give the reader a clear next step after completing the guide instead of ending with theory.

**Sources:**

- NIST CFReDS – *Hacking Case*
- CyberDefenders – *Blue Team Labs*

---

## From Curation to Synthesis

The DFIR Field Guide created during Project 01 answered the question:

**"Where can someone beginning DFIR find reliable resources, tools, and training?"**

This synthesis project asks a different question:

**"How does a Digital Forensics and Incident Response investigation actually work?"**

The resources from the original collection will support the new product, but the organization will no longer be based primarily on categories of resources. Instead, the information will be reorganized around the investigative process.

The finished product will guide a beginner through the progression from recognizing an incident to preserving evidence, examining artifacts, interpreting attacker behavior, and developing practical investigative skills.

---

## Project Connections

This project is part of a larger collection of work documenting my development in Digital Forensics and Incident Response.

**Project 01:**  
[DFIR Field Guide](https://lorenzojvillalobos.github.io/dfir-field-guide/)

**Project 02:**  
DFIR First Steps: A Beginner's Investigation Roadmap  
*Final project link will be added when completed.*

**Professional Portfolio:**  
[Lorenzo Villalobos – Professional Portfolio](https://lorenzojvillalobos.github.io/professional-portfolio/)

---

[← Return to DFIR Field Guide](https://lorenzojvillalobos.github.io/dfir-field-guide/)  
[← Return to Professional Portfolio](https://lorenzojvillalobos.github.io/professional-portfolio/)
