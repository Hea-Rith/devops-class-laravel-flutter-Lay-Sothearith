# DevOps Conception Class
**Student:** Lay Sothearith

## Lesson 2: My CI/CD Pipeline
- **Project:** MeetSpace Management System
- **Trigger:** Push to `feature/room/search-listing`
- **Feature:** "Search Available Room" from a Laravel API
- **Target:** Laravel staging server + Android testing device

### Pipeline design
Code -> Test -> Build -> Release -> Deploy
| Phase | Action | Details / Components | Person | Output | Mode |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **1. Code** | Commit API updates | **API:** `api/room/listing/search`<br>**Screen:** `RoomListSearch.dart` | Developer | Commit | Manual |
| **2. Test** | Check API | **API:** `api/room/listing/search`<br>**Screen:** `search list` | Developer | Test result | Auto |
| **3. Build** | Package API + APK | — | Developer | Artifacts | Auto |
| **4. Release**| Approve `v1.0.0` | — | Release Lead | Approved version | Manual |
| **5. Deploy** | Stage API; Install APK | — | Ops / Tester | Running app | Manual |
### Controls
- **On test/build failure:** Stop, fix, and retest | **Release approval by:** Project Manager / Lead Developer
- **After Deployment check:** API endpoint & Room search UI | **If it fails:** Roll back to previous stable release
- **Feedback for the next change:** Monitor and collect feedback, and plan the next code change

---

### Pipeline Diagram

![My Pipeline Diagram](Lay_Sothearith.png)
