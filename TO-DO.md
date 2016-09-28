FILTERING
=========
 - [ ] Add a NOT condition to filters
 - [ ] When making a filter subscription local, clear the ID so it doesn't show "subscription" in the list
 - [ ] Add CURRENT TIME and POST TIME to the list of conditions in filters
 - [ ] Make an example "Spoiler" filter for Game of Thrones that hides posts until Monday night
 - [ ] The "Replace" action only works once, adding another one doesn't replace the second case
 - [ ] New action: "Click Selector"
 - [ ] New action: "Hide Selector"
 - [ ] Add some way to alert users of new subscription filters and tweaks
 - [ ] Filter by post privacy level
 - [ ] Detect and warn about regex filters with a trailing |
 - [ ] New action: "Apply Style" with a pre-defined list of styles that can be applied, like "Red Outline"
 - [ ] Add a "Filter Posts Like This" option to the filter drop-down to help get quickly started on a filter
 - [ ] If a filter condition contains App or Author, add an item in the filter PAI to "add <author> to filter <x>" to easily add people to existing filters

HIGH
=========
 - [ ] When users have a gray icon next to their name (when not in a group, for example) the code for the icon is included in the tab name - https://www.facebook.com/groups/SocialFixerUserSupport/permalink/1074831415919072/

MEDIUM
=========
 - [ ] PAI's should be shown on single posts
 - [ ] Make the Options searchable
 - [ ] Add an option to make the wrench/control panel not draggable
 - [ ] The Display Tweak "Force Chat Popup To Default Colors" should also include: ._1nc6 ._d97 {background-color:#4080ff !important;}
 - [ ] Comment navigator "expand all" doesn't work consistently on all posts. ex: https://www.facebook.com/Stonekettle/posts/1097609370274465

LOW
=========
 - [ ] Post action icons don't appear on posts that get added under the cursor. The mouse needs to be moved out of the post and then back in for them to appear.
 - [ ] Add a separate option to show the filter icon / wrench icon, separate from the "Mark As Read" functionality
 - [ ] The control panel is partially hidden by the white strip at the top of Pages
 - [ ] Add content to the "About" tab
 - [ ] Allow users to define which groups/pages not to filter even if it's turned on
 - [ ] Show "Advanced" code view for Tweaks

UNPRIORITIZED
=============
 - [ ] "Anonymize Screen" does not anonymize friends names in chat toolbar at the right edge of the screen
 - [ ] "Anonymize Screen" does not anonymize friends names in Birthdays panel at top of right column
 - [ ] Option to change font size
 - [ ] Quick links (pages, groups)
 - [ ] Option to disable user hovercards
 - [ ] PAIs: option to adjust size/show all the time
 - [ ] Lock r. column tweak
 - [ ] R. click CP tab to make it open in a new browser tab
 - [ ] Shortcut to go to directly to Edit filter screen from post or CP
 - [ ] Shortcut to go to the Tweaks screen
 - [ ] KB shortcut for "mark as read"
 - [ ] When MAR read for a tab it goes to the next tab that has posts. When clicking Undo, it does correctly Undo "somewhere". I would like to request ability to jump back to the tab where posts were Undo. It might not be necessarily the one prior to the one you're currently on.
 - [ ] Add "Comment Navigator" to posts coming from Notifications

FUTURE IDEAS / FEATURES
=======================
 - [ ] Comment Button
 - [ ] Enlarge photos when hovering
 - [ ] "Timeout" feature for a friend, to hide their posts for a certain amount of time and be reminded to add them back
 - [ ] Configurable keyboard shortcuts
  
TECHNICAL
=========
 - [x] Trigger resize a couple times after clicking a tab, to trigger Facebook to show posts that were hidden
 - [ ] Add functionality to track daily user count and which filters/tweaks are most popular
 - [ ] If no posts are ever hidden/tabbed from filters or being marked read, don't throttle the post loading, because it will never run forever
 - [ ] When navigating, all posts marked as read get shown before page transition - only when clicking an item in notifications?
 - [ ] Add a debugger/page inspector option to allow users to report HTML structure
 - [ ] Minify Zepto
 - [ ] Figure out why injecting X into the page context breaks buttons on the "settings" page
 - [ ] Move "anonymizer" config to the server as a JSON configuration
 - [ ] Performance: Only call extract() on posts for data parts that actually have filters defined for them
 - [ ] Internal: Connect Facebook's Arbiter to X.publish() to listen to all their messages and take action
 - [ ] Switch to Vue 2.0 with pre-compiled templates
 - [ ] Update config*.json on the server to alert users of old versions about v15

FB WATCH
==========
 - [ ] Add more logging/debugging info
 - [ ] Redirect to a "clean" url after adding an item
 - [ ] Change the interval automatically - If new activity is found, check back more frequently
 - [ ] Update the Graph API version being used
 - [ ] Explained here: https://www.facebook.com/groups/551488248212943/permalink/1339012749460485/?comment_id=1339118706116556&comment_tracking=%7B%22tn%22%3A%22R2%22%7D
 - [ ] Add an additional column called "Age" or something along those lines. Premise is that with time discussions die down, so I would like to delete posts from Watch after let's say 20 days. Instead of going to each individual post to find out how old it is, I would to have this info in the grid.
 - [ ] Allow refresh rate value to be preserved if modified from defaulted 300
