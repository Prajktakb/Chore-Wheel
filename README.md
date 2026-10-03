# Chore-Wheel
• The annoyance
What it is: Passive-aggressive roommate friction and forgotten responsibilities over daily chores.
Who it annoys: College students and housemates living in shared apartments.
How I know: Personal experience living with 3 roommates and dealing with constant group chat arguments over dirty dishes and overflowing trash.
• Your constraint
Constraint: Offline-First PWA (Progressive Web App).
How it changed what I built: Architected the app using IndexedDB and a Service Worker cache so roommates can view, complete, and re-spin chores without internet. All actions queue up locally and sync to Supabase when internet returns.
• The great part
Which part: The Interactive Spinning Wheel chore distribution system.
Why: Gamifies household responsibilities and eliminates personal bias or arguments by randomly and fairly assigning chores across all roommates.
• The two testers
Tester 1 (Alex):

Where they got stuck: Could not find where to edit roommate names or add extra chores after finishing setup.

What I changed: Added a dedicated "Roommates" navigation tab for editing members and custom chores on the fly.

Tester 2 (Sam):

Where they got stuck: Unsure if chore checkmarks were saved while airplane mode was turned on.

What I changed: Added a live connection status badge (`🟢 Synced` / `🟠 Offline — Local Storage`) directly in the main header for clear visual feedback.

• AI
What AI was used for: Writing UI layout boilerplate, drafting Service Worker caching strategy, and calculating canvas rotation physics.
One thing AI got wrong: AI initially used standard `localStorage`, which failed during offline array operations; I refactored it to use a structured IndexedDB store and transaction queue.
• Not done
Push notifications for daily chore reminders.
Automated weekly auto-spin trigger every Sunday midnight.
