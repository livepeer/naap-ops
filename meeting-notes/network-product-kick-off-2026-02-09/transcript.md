## Network Product Team Sync - Transcript

**Date:** Feb 10, 2026

**Topics:** Network Product Vision, Team Roles, Meeting Cadence, Epics, Plugin Architecture, Development Workflow

---

**00:00:00 - Introduction and Recording Setup**
Qiang Han, Rich O'Grady, Mehrdad Sadeghi discuss recording initiation. Mehrdad starts Gemini for note-taking.

**00:00:49 - Technical Issues and Attendance Check**
Speedy Bird Tech mentions heating issues. Mike Zoop joins later, also facing heating problems. John Mull and Josh's attendance is confirmed.

**00:01:42 - Meeting Purpose and Introduction**
Rich O'Grady welcomes attendees, emphasizing the goal of aligning the cross-functional team on building the network product. He highlights the foundation's commitment to this critical ecosystem component.

**00:02:45 - Meeting Agenda**
Rich O'Grady outlines the agenda: team/product introductions, roles/responsibilities, timeline & epics, collaboration methods, and next steps. "Epics" are defined as collective goals for the network product team, distinct from individual group milestones.

**00:05:14 - Team Introductions**
*   **Rich O'Grady:** Focuses on growth and go-to-market for Livepeer.
*   **John Mull:** Orchestrator for four years, runs Elite Encoder node, developer with Livepeer.
*   **Qiang Han:** From the Inc. side, initiated the portal-based NA project.
*   **Mehrdad Sadeghi:** Ecosystem-wide PM, tracks foundation programs, previously involved with Raid Guild, Pocket Network.
*   **Speedy Bird Tech:** Orchestrator, software engineering background, working on data pipelines for observability.
*   **Mike Zoop:** Orchestrator, involved in Cloud SP proposals, software engineer, experience in large-scale systems.
*   **Pelina:** Marketing Manager (joining remotely), handles distribution and communications.

**00:07:35 - MVP One-Pager and Network Product Vision**
Rich O'Grady introduces the MVP one-pager as a single source of truth. The network product aims to be a central "shelling point" for developers to access network capabilities (gateways, transcoding, AI), enabling demand on the network. Key attributes: observable, performant, and user-centric.

**00:11:42 - Modular Architecture and Community Plugins**
The product is being built with a plug-in-based modular approach. The plan is to develop core plugins initially, with community development eventually taking over, positioning the platform like an app store.

**00:13:14 - Feedback on Vision**
Rich O'Grady solicits feedback on the product vision, with participants generally in agreement.

**00:14:47 - Roles and Responsibilities Clarification**
*   Mike Zoop and Speedy Bird Tech are identified as "Data Engineers" for clarity.
*   Josh's role in the SDK initiative is discussed; he shares a similar role to John Mull and works with Qiang Han.
*   Mike Zoop highlights the importance of consistent data sharing across groups for the cloud SP analytics platform and Qiang Han's dashboard.

**00:20:27 - Data Flow and Consistency**
Mike Zoop emphasizes that data needs to flow through the cloud SP analytics platform to feed the dashboard, stressing alignment on this point.

**00:21:31 - Josh Joins and SDK Development**
Josh joins the meeting. His role is described as working on the platform with John and Qiang Han. John Mull mentions needing to push changes to the SDK due to initial design limitations.

**00:23:38 - Network Product as a Shelling Point**
Rich O'Grady reiterates that the network product should be the central hub where ecosystem components converge, driving value to the Livepeer network.

**00:24:47 - Clarification on Technical Program Manager Role**
Qiang Han asks for clarification on Mehrdad Sadeghi's TPM role. Mehrdad explains it as the "operational glue," ensuring tasks and deliverables are met and preventing blockers.

**00:26:13 - QA and Accountability**
Rich O'Grady clarifies his role in product QA and go-to-market readiness. Mehrdad's role is to ensure the group remains accountable and that milestones are shipped.

**00:27:25 - CI/CD and Plugin Builder Collaboration**
John Mull expresses the need for end-to-end quality assurance in CI/CD and operational excellence, inquiring about working with plugin builders.

**00:28:27 - Plugin Definition Discussion**
John Mull raises questions about the definition of a "plugin" and the SDK being a client application. Rich O'Grady postpones this vital discussion to avoid diverging opinions, suggesting Qiang Han prepare pre-reading material.

**00:31:18 - Network Product Epics**
Rich O'Grady defines three collective "epics" for the team:
1.  **Foundational Metrics and Platform:** Achieve observability and a dashboard by the end of February.
2.  **Network MVP Public Launch:** Publicly launch the MVP with core plugins, a dashboard, plugin lifecycle management, and integrated observable data.
3.  **Community Plugins:** Integrate the first community-built plugins to enable demand on the network.

**00:35:51 - Need for Plugin Clarity**
John Mull, Speedy Bird Tech, and Josh express a need for more clarity on core plugins, their value, and technical implementation. Speedy Bird Tech notes confusion about the core concepts and technical design of plugins. Josh suggests using "features" instead of "plugins."

**00:39:32 - Plugin Definition Discussion Postponed (Again)**
Rich O'Grady agrees a follow-up discussion on plugins is necessary, proposing a dedicated meeting on Thursday. Qiang Han will prepare pre-reading material on the plug-in architecture, types, and initial core plugins. Qiang Han clarifies the MVP is a portal to surface existing network services, not invent new ones.

**00:50:00 - Administrative and Operational Updates**
*   **Weekly Sync:** Proposed weekly sync meeting every Tuesday at 5:00 p.m. GMT for 30 minutes, run by Mehrdad Sadeghi.
*   **Glossary:** Rich O'Grady and Mehrdad Sadeghi will create a public glossary on GitHub.
*   **Communication:** Moving communications from DMs to public channels and GitHub for project updates, milestones, and issues.
*   **GitHub for Planning:** Emphasized using GitHub for planning and updates, promoting asynchronous communication.

**00:53:35 - GitHub Project Management Demo**
Mehrdad Sadeghi demonstrates using GitHub milestones for project tracking, highlighting its public nature and AI integration potential.

**00:56:17 - Iterative Planning on GitHub**
Discussion on how iterative planning will work via GitHub issues and asynchronous communication. Individual engineering teams will hold their own weekly planning standups.

**00:58:47 - Process Management and Milestones**
Mehrdad Sadeghi outlines collaborative process management, with teams creating issues and committing them to milestones, and Mehrdad managing milestones across verticals for harmony. A follow-up call will be scheduled to set up details for Epic 1.

**00:59:44 - Technical Specifications and Documentation**
John Mull suggests tech specs or design calls as artifacts feeding into issue creation. Qiang Han agrees to share relevant documents on GitHub.

**01:01:06 - Next Steps Review**
*   Rich O'Grady to schedule a meeting for Thursday to discuss "plugins."
*   Weekly syncs on Tuesdays at 5:00 p.m. GMT to start next Tuesday.
*   Rich O'Grady and Mehrdad Sadeghi to work on a glossary.
*   Rich O'Grady and Qiang Han to prepare pre-reading material and core plugin lists for Thursday.
*   John Mull and the group to work on design aspects.

**01:03:42 - Transcription Ended**