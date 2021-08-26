# Super-Template v1.2.0

The Super-Template objective to simplify slot game development. It still in early stage development and release, so it may contain bugs and a lot stuff to improvement. It will do update every **2-4 weeks**. Any issue and feedback are welcome to let us know.

---

Super-template subject to change from time to time when:

- New game requirement or changes request
- Super-Template improvement or bugs fix
- To-do list

## Update

### v1.2.0 (26-August-2021) [download patch here](https://github.com/GT3-Game/super-template-update-files/tree/main/update)

[v1.2.0 Update guideline](contents/version-release/version-release.md)

- Added API interation
- Added Login Page
- Added GameSetting.ts
- Added brand switching handler. URL.com/?br=kiss918 or URL.com/?br=Mega888. Default using Mega.
- Added local testing or real API switching
- Added error message pop up
- Added property to control reel stop speed
- Added cocos_inspector_lite extension
- Added res_compress extension
- Fixed AudioManager cannot resume play SFX after pause
- Fixed HUD balance update problem
- Update GameServer.ts
- Update bet per line paramater passing
- Update last reel spin delay
- Combine same winning line into one
- Bugs fixed

Known issues to fix in Super-Template

- When combine same winning, bottom wining message also need to combine (for both way game) [issues link](https://github.com/GT3-Game/super-template-docs/blob/main/contents/video/issues/FlowFor2LineWinIsWrong.mp4)
- When using auto spin, spin button should enable back immediately when reel stop [issues link](https://github.com/GT3-Game/super-template-docs/blob/main/contents/video/issues/SpinEnableDelay.mp4)
- Dollar ball information panel should hide when dollaball is disable

[v1.2.0 Update guideline](./contents/version-release/version-release.md)

### Note

To avoid confusing, we have make some changes.

1. 'modules-bundle' folder remain in project for reference. (may copy from super-template if deleted)
2. Bonus game need develop in your project.
3. Gamble game need develop in your project. (you may reuse gamble game prefab in 'modules-bundle')
4. Version update files can get it from here. https://github.com/GT3-Game/super-template-docs/tree/main/resources/cocos-creator/update
5. For on development project, current need to manually update. Which is get latest patch from Git, and merge code changes by using tools such as BeyondCompare.
6. if you are starting from fresh, can directly get latest super-template.

### v1.1.2 (6-August-2021) [download patch here](https://github.com/GT3-Game/super-template-update-files/tree/main/update)

- Revert "Remove 'modules-bundle'" (may copy from super-template if deleted)
- Added ProgressiveJackpotPrefab localize
- Added slightly delay when spin end
- Fixed auto adjust Betline and BetDenom issue
- Fixed reel spinning issues when spam click with single reel and play button
- Update 'swipe and spin' emit event name

### v1.1.1 (3-August-2021) [download patch here](https://github.com/GT3-Game/super-template-update-files/tree/main/update)

- Added modules-config.json handler
- Added Insufficient Balance Message
- Added GlobaData.ts
- Fixed issue when showing help-information panel still able to spin using keyboard space key
- Fixed Incorrect Balance Display
- Fixed Post big win sfx need to cut when reset function apply
- Remove 'modules-bundle' folder
- Update API http to https

### v1.1.0 (12-July-2021) [download patch here](https://github.com/GT3-Game/super-template-update-files/tree/main/update)

- Added Dynamic Modules Loader
- Added Fullsceeen Control
- Added GameServer Manager to Call API
- Update Swipe and Spin Feature
- Bugs Fixed
- Super-Template now separate and hosting `modules-bundle` with another project.
- Every module inside `modules-bundle` will get through http request.
- `modules-bundle` now will maintain by GT3 team.
