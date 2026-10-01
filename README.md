# DevOps Conception Class
- Student: [Name]

## Lesson 2: My CI/CD pipeline
- Project: [Flutter app + Laravel API]
- Trigger: [Push to practice branch]
- Target: [Staging + test device]

### Pipeline design
Code -> Test -> Build -> Release -> Deploy
1. Code: [action] | [person] | [output] | [auto/manual]
2. Test: [action] | [person] | [output] | [auto/manual]
3. Build: [action] | [person] | [output] | [auto/manual]
4. Release: [action] | [person] | [output] | [auto/manual]
5. Deploy: [action] | [person] | [output] | [auto/manual]
### Controls
On test/build failure: ... | Release approval by: ...
After deployment, check: ... | If it fails: ...
Feedback for the next change: ...
Optional drawing: ![My pipeline](pipeline.png)
