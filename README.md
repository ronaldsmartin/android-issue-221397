# android-issue-221397

**Update:** The Android team has categorized this issue as a defect and passed on the issue to the Support Library team as of October 17, 2016. Thanks to them for their work.

In the meantime, you can avoid this issue on your Floating Action Buttons by using standard `layout_margin`s instead of combining the `layout_anchor` and `useCompatPadding` styleable attributes.

## About

This project reproduces a `CoordinatorLayout` bug in Design Support Lib v24.2.x in which `layout_anchor`ing does not stick as well as it should.

## Steps to reproduce

1. Press the FAB. 

The Snackbar comes up and the FAB's padding is lost.  After a few seconds, the padding returns and the FAB moves to the correct position.

(The expected behavior is that the padding is consistent across the entire Snackbar animation.)
