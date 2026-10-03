# Chore-Wheel

• The annoyance :

What it is: Passive-aggressive roommate friction and forgotten responsibilities over daily chores.
Who it annoys: College students and housemates living in shared apartments.
How I know: Personal experience living with 3 roommates and dealing with constant group chat arguments over dirty dishes and overflowing trash.

• My constraint :
Constraint: Offline-First PWA (Progressive Web App).
How it changed what I built: Architected the app using IndexedDB and a Service Worker cache so roommates can view, complete, and re-spin chores without internet. All actions queue up locally and sync to Supabase when internet returns.

• The great part :
Which part: The Interactive Spinning Wheel chore distribution system.
Why: Gamifies household responsibilities and eliminates personal bias or arguments by randomly and fairly assigning chores across all roommates.

• The two testers
Tester 1 (Sharvari):

Where she got stuck: Could not find where to edit roommate names or add extra chores after finishing setup.

What I changed: Added a dedicated "Roommates" navigation tab for editing members and custom chores on the fly.

Tester 2 (Vaishnavi):

Where she got stuck: Unsure if chore checkmarks were saved while airplane mode was turned on.

What I changed: Added a live connection status badge (`🟢 Synced` / `🟠 Offline — Local Storage`) directly in the main header for clear visual feedback.

• AI :
What AI was used for: Writing UI layout boilerplate, drafting Service Worker caching strategy, and calculating canvas rotation physics.
One thing AI got wrong: AI initially used standard `localStorage`, which failed during offline array operations; I refactored it to use a structured IndexedDB store and transaction queue.

• Not done
Push notifications for daily chore reminders.
Automated weekly auto-spin trigger every Sunday midnight.

1.Dashboard : 
<img width="799" height="471" alt="image" src="https://github.com/user-attachments/assets/e96e8d21-2e56-4420-93aa-06a68c51817c" />

2. Schedule :
   <img width="824" height="543" alt="image" src="https://github.com/user-attachments/assets/d4e5a977-2e6b-4db2-a733-9682cbb14ade" />
   
3. Fun Spin wheel :
   <img width="447" height="399" alt="image" src="https://github.com/user-attachments/assets/6c15565d-34a7-484d-902d-d1678211132f" />

4. Roommates and Chores Page :
   <img width="817" height="417" alt="image" src="https://github.com/user-attachments/assets/bf955437-6f2f-4713-bd45-bb759fefc377" />




