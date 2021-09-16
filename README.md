# As note

Advanced bookmark manager for chromium.
Consider bookmarks as notes.
Tab management as onetab, but use bookmarks as backend.

## Features

- Integrated with native bookmark system.
- Tags.
- Sticky notes in web page.
- The key features of onetab.
- Advanced bookmark management.
- Auto sync.
- Export a single bookmark folder.
- Trash and Recycle mode
- Picking mode
- Shortkeys

## Concepts

### node

A node is a bookmark or a bookmark folder in Chromium.

### home folder node

The Home folder is the working bookmark folder of AsNote. By this you can let AsNote load only one folder.

### inbox folder node

Newly created bookmarks will be put into the subfolders of inbox folder. If there is no inbox folder appoited, home folder will be used as inbox.

### Trash

When in 'Trash' mode, all deleted nodes will be marked as trash and moved into trash folder. You can restore them by 'Normalize' function.

You should select a trash folder node to enable trash mode. Any folder may be appoited as trash folder, even outside of working folder.

### Recycle

'Recycle' engine may reuse these 'trash' nodes when you create new nodes.

'Recycle' is designd to reuse node ids. Generally this is not necessary if you do not know what it is. So it is disabled by default.

### Picking mode

Suppose you are viewing a page contains many links. You want to mark some of the links and read them another day. This is what we called "link picking".

After switched to Picking mode, any links clicked with 'Ctrl' in that page will be bookmarked and the openning of new tabs will be terminated. You can click any other tab to exit Picking mode.

### onetab

A 'tab' in onetab is nothing but a bookmark node in Asnote.

Save [one tab] / [all the tabs] / [tabs on the right] to inbox folder and close these tabs.

In app page, you can reopen these tabs/bookmarks by click the titles. But if you click the urls on the right side, the node will be removed at the same time. This is what we called 'restore'.

AsNote is designed for large data. You can save thousands of tabs without any trouble. Your data's safety is guaranteed by your native bookmark system.

### [Fold] (toolbar)

'Fold' creates a new folder besides the last selected node and moves all selected nodes into that folder.

Suppose you want to move several nodes into a folder.

### [Merge] (toolbar)

'Merge' unfolds all other selected folders(if they are folders) and moves them into(or beside) the last selected node.

'Merge' is designed to merge several folders but it is also useful for bookmarks.

## Tips

Select multi folders with 'Ctrl'.

Move url nodes with [merge].

Remove marks of trash with 'normalize'.

## FAQ

### Why do asnote need permmision of "Site access On all sites"?

This is necessary only if you want to show sticky notes in web pages automatically. You can disable it if you want. This will not affect any other features.

### How to import data?

AsNote is just bookmarks.
You can use your native bookmark manager to import bookmarks.

### May I import onetab's data to AsNote?

Yes.

You can import onetab's export data into bookmarks directly.

But the onetab's default export data has no folder/time information. We write a little exporter to parse and download it as bookmarks:

<https://raw.githubusercontent.com/asnote/help/main/onetab-exporter.js>)

1. open the onetab page in your browser.
2. open the 'developer tools' panel of your browser. (Ctrl+Shif+i)
3. click 'console' tab of the 'developer tools'.
4. copy our codes and paste them into 'console'.
5. press 'enter' key.

That's all.
