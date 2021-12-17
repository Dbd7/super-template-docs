# Super-Template v1.4.0

The Super-Template objective to simplify slot game development. It still in early stage development and release, so it may contain bugs and a lot stuff to improvement. It will do update every **2-4 weeks**. Any issue and feedback are welcome to let us know.

---

Super-template subject to change from time to time when:

- New game requirement or changes request
- Super-Template improvement or bugs fix
- To-do list

## Update

### v1.4.0 (17-December-2021) [download patch here](https://github.com/GT3-Game/super-template-update-files/tree/main/update)

- Added dynamic faviconURL
- Added new language code handler
- Added maintanance code
- Added UAT requirement update
- Update RunningNumberLabel.ts
- Update brand name from Mega888 to X500
- Update convertOptionpoIntoWinningLineFormat logic
- Update HUDSwipeDetectorComponent
- Optimize game launch speed

### v1.3.0 (25-October-2021) [download patch here](https://github.com/GT3-Game/super-template-update-files/tree/main/update)

##### (Change version to 1.3.0 for more correct increment)

- Added DomainManager (Dynamic get API URL by BrandCode. Default is mega branch, use ?br=kiss91 change to 918 brand. Please use relative player account to login)
- Added CryptoManager
- Added q parameter support login
- Added Jackpot API (server side only, local/custom pending)
- Update new scatter payout data structure
- Update Empty URL Handler
- Update GameSetting.ts (S)
- Update login API to version 2
- Fixed pop up clickable behind reel
- Fixed incorrect spin button show in auto spin mode
- Fixed SymbolMappingName to winning line

### v1.2.1 (29-September-2021) [download patch here](https://github.com/GT3-Game/super-template-update-files/tree/main/update)

- Added dynamic loading page. Show different loading by brand
- Added hide extra symbol when reel stopped function
- Added support to latest Mega888 and kiss918 bigwin
- Added sync new balance with API
- Added Scatter payout winning handle (S) [link](https://github.com/GT3-Game/super-template-outsource/commit/930bbc587f899c6d0ecd405290b00ad80ed2f577)
- Added dollar-ball and gamble game checking
- Added Random symbol result when show game screen
- Added currency code display (S) [link](https://github.com/GT3-Game/super-template-outsource/commit/c1c1102fbcab3766023fa4c5e923ba1007615452)
- Added blur sysbom control in GameSetting.ts and SlotReelStripPrefab.ts (S) [link1](https://github.com/GT3-Game/super-template-outsource/commit/b4f3f6aa71d5cec763b3d7c0c4552697a83a890a) [link2](https://github.com/GT3-Game/super-template-outsource/commit/c1b66a3d110e38a910fb5baf020cd32cab6008a1)
- Added control DollaBallGroup position
- Added Logout API
- Added symbol array

- Update mega and 918 config
- Update GameSetting.ts (S) [link](https://github.com/GT3-Game/super-template-outsource/commit/b4f3f6aa71d5cec763b3d7c0c4552697a83a890a)
- Update paylinerid to paylrnum in GameServerModel.ts
- Update bankCounter logic
- Update winning line animation (S) [link](https://github.com/GT3-Game/super-template-outsource/commit/3156b51101785aa9e9c08ed90eb862025adb9d29)
- Update LoadingPanelPrefab UI
- Update API HTTP error code
- Update png-auto-compress setting

- Fixed reel re-spin issues
- Fixed auto spin issues
- Fixed display amount issues
- Fixed duplicated API call
- Fixed incorrect last reel index
- Fixed min matched symbol for calculate winning line

- (S) need special take care, it might conflict

### Minor Hotfix Update (8-September-2021)

If you facing those issues, may update in your current project now.

[Details](contents/update/update.md)

- BigWinAnim Script (Mega888 only) on server, if facing any issues on bigwin like hide/show button, sound no stop or close bigwin animation. Can reference files here. [Download](https://github.com/GT3-Game/super-template-update-files/tree/main/others/BigWinAnim/8-August-2021)
- Result wining line return NaN issue [Link](https://github.com/GT3-Game/super-template-outsource/commit/bc8959a065349877869774a12cb0ec4c65691218)
- Duplicate API call [Link](https://github.com/GT3-Game/super-template-outsource/commit/53c7371bbd86779c39d90027ded4bab96346893c)

[Details](contents/update/update.md)

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
