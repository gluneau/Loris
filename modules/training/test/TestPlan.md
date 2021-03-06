# Training module test plan:

1. Check for Training item in the Clinical menu.
 a) If current user has 'training' permission, menu item should be there.
 b) If current user does not have 'training' permission, menu item should not be there.
2. Check for Training permissions (called 'training') in the user accounts section.
3. Does Training module load when clicking menu item?
4. On training page, tests are loaded to appropriate lists (certification completed or not completed).
5. Opening a test expands to full test view.
6. Click accept button and review training content, check that each type of content is display.
 - Text/html content
 - Pdf content
 - Video content
 - Quiz content
7. Quiz testing
 a) Quiz section can be filled out and submitted
 b) If user fails the quiz, should see pop-up to choose next action.
 c) If user passes quiz, they see pop-up saying they are certified.
8. Completion of certification grants permission to administer instrument - check on the Examiner page.
9. Adding more <CertificationInstruments> in the config.xml is required to appear in the training section,
    as instruments requiring certification. Verify that config.xml settings work as expected.
10. Adding new test: import SQL and copy pdf and mp4 files to project/data/training/ directory.
 a) See module Readme for example SQL content to import for adding new training and quiz.
 b) Media files (pdf, mp4) must have the same name as the test_name in order to display.
    Verify that this requirement works as expected.