# Manual test cases

| ID | Test | Expected result |
|---|---|---|
| T01 | Open `index.html` on desktop | Hero, directory, eligibility guide, and FAQ assistant render |
| T02 | Search `student` | Student-related sample entries remain |
| T03 | Select category `Health` | Only Health category entry remains |
| T04 | Select audience `Farmers` | Farmer support entry remains |
| T05 | Click `Reset filters` | Search and filters clear; all entries return |
| T06 | Open a scheme detail | Modal shows its illustrative description and safety reminders |
| T07 | Submit eligibility guide without required choices | Helpful validation message appears |
| T08 | Select student + age group and submit | Education/training discovery suggestions appear |
| T09 | Ask “How do I verify a scheme?” | Assistant advises official-source verification |
| T10 | Click language toggle | Hero copy and search placeholder switch to Hindi/English |
| T11 | Resize to mobile width | Layout stacks and remains usable |
| T12 | Inspect network/storage | No API calls or personal data persistence in this prototype |
