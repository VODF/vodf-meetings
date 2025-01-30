# Meeting of 2025-01-30

Present: Jutta, Laura, Karl, Bruno

[[TOC]]

# General context (BK)
- The `High Energy Interest Group` of [IVOA](https://ivoa.net/) has been recently created (see its 
  [Wiki](https://wiki.ivoa.net/twiki/bin/view/IVOA/HEGroup)). The 2025 roadmap focuses on an HE extension of ObsCore for
  the DL3/L1 (first semester) and the DL5.
- The SWGO dev team is actively working on the serialization scheme of their DL3/L1. These data will contain `event-type`
  flag for each event. A format is then needed and prototyping has been started.
- CTAO is planning to openly release simulated data in Spring 2026 for its Science Data Challenge. The data will contain  
  `event-type` flag for each event. A VODF format could be used, GADF format being a backup plan.

# General tools (KK)
- Presentation of the central tool providing self-documenting schema definitions: 
  [vodf-schema](https://github.com/VODF/vodf_schema) 
- After having made a survey of many tools (including JSON schema with Pydantic, JWST tool), it is based on the GADF tool
 [fits_schema](https://github.com/VODF/vodf_schema).
- Need to add validation utilities, sphinx plugin for the web documentation

# Work organization 
- We agree to focus on the DL3/L1 drafting first
- Strategy: writing of a coherent draft on the main aspects of the DL3/L1 between the LEs, and then discussions with
  other experts, then with the community
- Working methodology: 
  - proposal of modifications/writing with a PR
  - exchanges on GitHub
  - if a topic is complex, discussion during a remote meeting
- Need a F2F meeting to make significant progress
  - Possible slots: Feb 17..21, March 19..21 ir 26..28 (others?)
  - Location: MPIK (ECAP?)

# Discussion on the handling of `event-types`
- Introduction of the HDU hierarchy for event level data: see [design issue #1](https://github.com/VODF/vodf_schema/issues/1)
- It seems that there is an apparent difference between the CTAO plan and the SWGO one

# Action items
- [ ] Inform the Steering Committee of the current work - Karl
- [ ] Creation of a pool to find the date for the LEs F2F meeting - Laura
- [ ] Improve the general tools to allow editing - Karl
- [x] Set up of the meeting pages - Bruno
- [ ] Distribution of format items/parts that are not controversial to start the editing - Karl
- [ ] Try to reconcile the CTAO and SWGO HDU hierarchy for Feb. 7- Karl & Bruno