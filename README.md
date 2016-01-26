# showTrelloCardNumbers
Bookmarklet that shows the numbers of [Trello](http://trello.com/) cards.

![Numbered card sample](Trello-Card-Numbers.png)

#### Bookmarklet

+ Drag the link below to your browser bar (to create a bookmarklet):
  - [Show Trello Card Numbers](http://www.replace_this_entire_url_with_js_code.com)
+ Right Click on bookmarklet and choose Edit
+ Paste the JavaScript code below into the URL for the bookmarklet
+ Visit your Trello page to test the bookmarklet

```javascript
javascript:!function(){var o=$(".card-short-id");o.each(function(){$(this).text($(this).text().replace("#", ""))});o.hasClass("hide")?o.removeClass("hide").css({"font-weight":"normal","font-size":".8em","margin-right":"5px",padding:"2.3px 6px",background:$("body").css("background-color"),"border-radius":"10px",color:"#f6f6f6"}):o.addClass("hide")}();
```
