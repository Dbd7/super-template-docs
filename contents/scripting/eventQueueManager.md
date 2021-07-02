# EventQueueManager

Manage and controling UI event happening and resove it by sequence. Use it where you need it.

## Overall Idea

Create a EventQueue with `EventQueueManager`, stack event inside and resolve it by order of *LastTofirst* or *FirsToLast*.
So all event can easily resolve by spin button.

Spin button and space button use case:

1. Create EventQueue with name *SpaceOrSpinButton*
       EventQueueManager.getInstance().createEventQueue('SpaceOrSpinButton');

2. Added event inside *SpaceOrSpinButton* EventQueue
       // addEvent param ('EventQueue Name', 'EventId', 'Event Callback')
       // Add event btnSpinClicked (spin button)

       EventQueueManager.getInstance().addEvent('SpaceOrSpinButton', 'btnSpinClicked', () => {
            // do something here
            callSpin();
       });

3. When showing BigWin Animation, add event inside *SpaceOrSpinButton* EventQueue
       // Add event showBigWinEvent (when big win animation show up)

       EventQueueManager.getInstance().addEvent('SpaceOrSpinButton', 'showBigWinEvent', () => {
           // do something here
            hideSpin();
       });

4. Visualize *SpaceOrSpinButton* EventQueue

|index | Event Queue   |
|----- | ------------- |
|<div style="text-align:center">1</div>     |<div style="text-align:center">showBigWinEvent</div> |
|<div style="text-align:center">0</div>      |<div style="text-align:center">btnSpinEvent</div> |

5. Resolve event by click spin button or space button
        // Since resolve order is by 'LastToFirst'. So, index 1 - showBigWinEvent will mark as resolve and remove from EventQueue

        EventQueueManager.getInstance().resolveEvent('SpaceOrSpinButton', 'LastToFirst');
        

6. Remember to remove it after no longer use to prevent duplicate event
        // Need to remove from EventQuene if no longer using

        EventQueueManager.getInstance().removeEventById('SpaceOrSpinButton', 'ShowBigWinAnim');

## Conclusion

`EventQueueManager` use to helping resolve UI stack happening and what to do in sequence without complicated cross checking.
