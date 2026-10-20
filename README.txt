OT Documentation Updated — 20 October 2026

OPEN THE APP
For a single-file app, open OT-documentation-webapp-standalone.html in your browser. Its styles, scripts and icons are embedded; keep this filename when replacing an older standalone copy.

For the hosted/installable app, use index.html with app.js, phraseBank.js, style.css, sw.js, manifest.webmanifest and the icons folder together. Serve the folder over HTTPS or localhost for offline installation. The service-worker cache is version v109. Reload the app after deploying the replacement files.

CHANGES
• Bathing: Stand appears even when no bathing facility is selected.
• Home Help Service includes Exercise with a remarks field wherever the shared Social History form is used.
• Home O2 Assessment includes an editable, copyable Green Box in Summary, linked to Oxygen regime and Treatment plan. It retains the existing 250-character warning and does not truncate the note.
• Emergency Medicine is available in the assessment selector with nine sections based on ADL Initial.
• Premorbid Cognitive Function has free text and Unremarkable; Behavioral Problem has Nil/Yes and conditional details.
• AMT and Clock Drawing Test are always displayed in Emergency Medicine, with Unable to assess. MoCA opens through Done.
• Mood supports one primary choice plus Others and free text. Performed opens the 15 GDS questions and automatic scoring.
• GDS question 4 is “你常常感到生活沉悶嗎？”, as confirmed. Question wording, score keys and summary cutoff text otherwise follow the supplied specification.
• Chinese Lawton IADL includes nine items scored 0–3, a total out of 27, optional explanations, and item scores in Summary. NA means not assessed.
• Each GDS and Lawton item occupies its own full-width row. GDS response buttons sit alongside the item on wider screens and below it on smaller screens.
• Lawton follows the MBI card format: item title and a Not assessed / score pill above a full-width row of NA, 0, 1, 2 and 3 buttons. NA is highlighted when no score is recorded; optional item explanations appear below the buttons.
• Unfinished Lawton assessments show “>= xx/27, pending further assessment” in the form and Summary, where xx is the sum of assessed items. Completed assessments show their final score out of 27.
• When GDS is marked Performed, a reminder in the form and Summary asks the therapist to answer all 15 questions. The total score appears only when all questions are answered.
• Unfinished AMT summaries show “AMT: pending”, including linked OT comments and the Green Box. Unfinished summaries omit answered-count and subtotal brackets. Blank answers are not treated as zero.
• Emergency Medicine fall history supports multiple incidents and multiple reasons per incident.
• Emergency Medicine uses “Continue 1-2 days ward-based training”. Other assessment forms retain their existing recommendation wording.

SAVED CASES
The existing local browser autosave and seven-day retention behavior remain in place. New fields are added when older saved records load. Case data belongs to the browser/site (or local file location); it is not included in these application files. A different browser, website address or local file location may use separate storage.

VERIFICATION
JavaScript syntax checks and 13 automated behavior checks passed, covering every form’s rendering, new scoring and text fields, conditional controls, summary output, Home O2 Green Box synchronization and saved-case compatibility. Browser checks confirmed Emergency Medicine, the revised GDS question and 9/15 result, Lawton 9/27, Exercise remarks, Bathing: Stand and the linked Home O2 Green Box. The standalone build uses the same scripts and styles as the folder version.
