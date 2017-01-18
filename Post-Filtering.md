(This page is a work in progress!)

<h1 id="filter-list">Filter List</h1>

## Active Filters

The top list of filters are those subscriptions that you've added and any filters you've created yourself. Each post in your news feed will be processed be each filter in this list, in order. 

The order of filters matters because filters can run and stop the execution of subsequent filters. For example, your first filter might hide a post, and a lower filter may move it to a tab. But if it's hidden, you don't want it to also be moved to a tab.

The "Stop on Match" controls this behavior. If checked for a filter, then if it matches, any filters below will not be run on the post. This gives you ultimate control over how posts are handled.

The "Enabled" checkbox controls whether the filter actually runs. If not enabled, then the filter is skipped. This is useful for debugging or for temporarily removing a certain filter for a while.

## Filter Subscriptions

This is a list of pre-defined filters that are available for you to add. To make a subscript Active, click the plus icon on the right, which will make it appear in the list above.

Subscription filter definitions are updated automatically. So if Facebook changes their code or if new terms need to be added to the filter to keep it working as expected, you don't need to do anything. The subscription will automatically be updated in your list. Subscription filters in the Active list show the date when they were last updated.

<h1 id="edit-filter">Edit Filter</h1>

IF a post matches the conditions, THEN actions are taken on it. That's the basics of post filtering.

## IF

Define one or more conditions that define whether a post matches. First pick which part of the post your condition matches against, then what you want to test.

 - Any Post Content
   - Contains
   - Equals Exactly
   - Starts With
   - Ends With
   - Matches Regex : Define a regular expression to match against the content. Don't include the / at the start or end. Include modifiers like 'i' for case-insensitivity in the second box. A testing util is included if you wish to try out your regular expression to see what it will match.
   - Matches CSS Selector
 - Post Text Content
 - Post Actions
 - Author
 - App/Game Name
 - Link URL
 - Link Text
 - Day of the Week
 - Post Age
 - Picture Of

## THEN

Decide what action(s) to take to posts that match the IF conditions.

 - Hide Post
   - Show Message
 - Add CSS
   - To Selector
 - Add CSS Class
 - Replace Text
 - Most post to tab
 - Copy post to tab

### Advanced Code


