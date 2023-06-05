# Discovery
The data has been loaded into a BigQuery instance and connected to the following Count Canvas: https://count.co/canvas/SNoES0y3yvd (can be accessed but not edited).

## Raw Data
List of documents:
- Artifacts-P1.pdf
- Artifacts-P2.pdf
- Artifacts-P3.pdf
- Loss-P1.pdf
- Recent-Developments-P1.pdf

List of data files:
- actions.csv
- divisions.csv
- employees.csv
- managers.csv
- safehouses.csv

### Artifacts-P1.pdf
Multiple words throughout the document are redacted.
References to Artifact One, Artifact Two and Artifact Three.
Artifacts are mostly identical, Two has a focus on `[REDACTED-INIT]` and Three most likely is the most powerful of them.

### Artifacts-P2.pdf
Multiple words throughout the document are redacted.
References a database with details, analysis and intelligence.
Violations of this policy will be dealt with via BRLDA directive 119-393a protocol (unknown what this entails).
Additional Notes are entirely redacted.
Signed by "Director, Bureau of Really Large Data Analysis".
`End of Briefing Document` is printed at the bottom.

### Artifacts-P3.pdf
Multiple words throughout the document are redacted.
References `Appendix I: Device Schematics`.
Devices One and Two are retro-style handheld devices. 7.9" widescreen display, 1280x400 resolution. 48-key ortholinear mechanical keyboard. 
Device Three references Artifact Two being a 5" round screen, with a keyboard and case of some kind.

### Loss-P1.pdf
Some words in the document are redacted, but less than in Artifacts-P1 through Artifacts-P3.
References that the Artifacts are 2 months old.
Betrayal was done through field operatives of the BRLDA. The operatives deleted references to themselves in the databases.
Artifacts were located in a safe house, which due to the data erasure is now location unknown. Likely the artifacts were taken by the operatives outside the safe house.
Inside BRLDA is a strict information blackout while they investigate.

### Recent-Developments-P1.pdf
Some words in the document are redacted.
Reference to three (3) devices, which are described in another document in Section 18f.
Tracking down the devices has been a multi-year effort with no reward.
One of the devices is the most elusive of all three, with very few sightings. 
In 2023 (exact date is redacted) field operatives secured all 3 artifacts (devices) in a safe house. ```The safe house was later compromised, referenced in Loss-P1.pdf```

### divisions.csv
- 26849 rows

### employees.csv
- 26844 rows

### managers.csv
- 3836 rows

### safehouses.csv
- 202 rows

### actions.csv
- 97391 rows

# Known Facts
## Documents
- Artifacts === Devices
- There are three (3) devices in circulation, of which one is the most "powerful" (uncertain of that exact meaning).
- The safe house where the devices were being held was compromised by field agents.
- The identities of the fields agents who went rogue are unknown and references or data were destroyed in the database(s).
## Data Exploration
- There are no safehouses where no employees are "attached".
- There are 5 employees aka "subjects" with actions who are not listed in the employees table (IDs: 1423, 4284, 14976, 22602, 26188). All subjects share the 219 safehouse (Ecuador) as their known safehouses.
- Our subjects are the only ones that did actions in the divisions 1, 3, 6, and 10 that weren't reflected in their employee record.
- There are 630 employees that did actions classified under Division 7 that don't have that division reflected in their employee record.
- The subjects' actions mention the three devices.
- Some duplicate employees are present in the data. Same email, but different phones and managers.
- Jessica Stone is the only manager without any employees.

# Open Questions
- Do the 630 employees with actions under Division 7 warrant further investigation?
- What information do we additionally want to retrieve about the 5 subjects?
- Is Jessica Stone (Manager with employees) relevant to the investigation?