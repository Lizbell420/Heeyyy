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
 - [ ] Disable Wrench under https://apps.facebook.com/*, which includes games.
 - [ ] Tab list gets created in Pages/Groups even if no filters are moving posts to tabs
 - [ ] Some Chrome users get storage errors
 - [ ] When users have a gray icon next to their name (when not in a group, for example) the code for the icon is included in the tab name - https://www.facebook.com/groups/SocialFixerUserSupport/permalink/1074831415919072/

MEDIUM
=========
 - [ ] PAI's should be shown on single posts
 - [ ] Make the Options searchable
 - [ ] Add an option to make the wrench/control panel not draggable
 - [ ] Add an option to restore the position of the control panel
 - [ ] The Display Tweak "Force Chat Popup To Default Colors" should also include: ._1nc6 ._d97 {background-color:#4080ff !important;}

LOW
=========
 - [ ] Post action icons don't appear on posts that get added under the cursor. The mouse needs to be moved out of the post and then back in for them to appear.
 - [ ] Add a separate option to show the filter icon / wrench icon, separate from the "Mark As Read" functionality
 - [x] Add an option to pre-populate the filter tab list based on all defined filters
 - [ ] The control panel is partially hidden by the white strip at the top of Pages
 - [ ] Add content to the "About" tab
 - [ ] Allow users to define which groups/pages not to filter even if it's turned on
 - [ ] Show "Advanced" code view for Tweaks

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
 - [x] Can I force news feed containers to never hide and height:auto or will that break Facebook's feed hiding algorithm?
 - [ ] Add padding to the browser/sfx version box in the Support Tab
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
 - [x] Add a login button if the popup doesn't get triggered automatically
 - [ ] Redirect to a "clean" url after adding an item
 - [ ] Change the interval automatically - If new activity is found, check back more frequently
 - [ ] Update the Graph API version being used
