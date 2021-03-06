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

 - **Any Post Content**
   - **Contains** : Enter plain text to look for in the content. This is NOT case-sensitive.
     - Use the pipe | character to separate multiple "OR" conditions. ex: mary|bob|joe would match if ANY of those three words is found.
     - **"Match partial words"** : By default, text matches only whole words. So, entering "bob" will not match "bobby". If you want to match parts of words (so "politic" would match "politics" and "political" for example), check this box.
   - **Equals Exactly**
   - **Starts With**
   - **Ends With**
   - **Matches Regex** : Define a regular expression to match against the content. Don't include the / at the start or end. Include modifiers like 'i' for case-insensitivity in the second box. A testing util is included if you wish to try out your regular expression to see what it will match.
   - **Matches CSS Selector** : Use CSS syntax to define a selector to test against the DOM of the post. If the selector matches a node in the post, the condition is met.
 - **Post Text Content** : The content text actually entered by the user. This would include their comment about a posted link, but not the content of the link itself.
 - **Post Actions** : The activity text at the top of the post, such as "Bob Jones commented on this".
 - **Author** : The user who the post is from or about
 - **App/Game Name** : If posted from an app or game, test against the app name. ex: "Instagram"
 - **Link URL** : If the post is an external link, this is the url of the link itself
 - **Link Text** : The title and description of an external link
 - **Day of the Week** : Select days of the week when this filter should be active. For example, you can create a filter that only runs on Sunday, to hide spoilers for a certain show until the next day
 - **Post Age** : Filter posts based on how old they are. Example: Highlight posts that are more than a week old.
 - **Picture Of** : Match the auto-generated text labels generated by Facebook for photos. At the moment this is somewhat unreliable because it's difficult to predict the labels that they will apply to photos. It is a good experimental feature.

## THEN

Decide what action(s) to take to posts that match the IF conditions.

 - **Hide Post** : Remove the post from the news feed
   - **Show Message** : If you want to be aware of which posts are hidden, enable this checkbox to make a small note appear where the post would have been. This note is clickable to view the post that was hidden.
 - **Add CSS** : Enter css rules to apply to the post container DIV. Because of Facebook's complex CSS, figuring out effective CSS can be difficult. A good place to start is outline. ex: "outline 2px solid orange;"
   - **To Selector** : Instead of applying the CSS to the post container, find a DOM node within the post and apply the CSS to that node instead. Ex: Highlight just the timestamp of posts that are older than 1 week
 - **Add CSS Class** : Add a class name to the post container node. This has no effect on its own, but should be used in conjunction with a Display Tweak that defines the CSS that uses the class.
 - **Replace Text** : Change the actual text content. Example: Replace swear words with "!#$"
 - **Move post to tab** : Remove the post from the news feed and put it in a "tab". The tab will appear in the control panel box. Clicking the tab name will show all posts in that tab and hide the others.
 - **Copy post to tab** : Instead of removing the post from the news feed, keep it in the main feed and also put it into the tab. Any actions taken on the post in one place will take effect in all. Posts can be copied to multiple tabs.

### Advanced Code

This box contains the internal JSON representation of the filter definition. It is useful for filter debugging, sharing filters, and directly editing filter definitions.

Pasting a filter definition into the Advanced Code box will populate the filter fields above. If the filter definition contains an error, the fields will not be populated.

