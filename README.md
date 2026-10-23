# Digital-Guest-Book
Digital Guestbook (방명록)

An interactive digital guestbook built for a university anniversary event. Visitors leave a handwritten or typed message, add stickers, take a photo, and submit. The latest 10 messages and photos then float across a large display as bubbles.

Interface language: Korean. English labels are given below for reference.

Guestbook writing screen

Overview

At the event, each visitor used a touch or mouse station to:

Pick a ribbon color for their message
Write or draw a message on the canvas
Add a sticker or emoji
Take a photo with the webcam
Press Register to publish it

Submitted entries appear on the big screen as animated bubbles. The screen always shows the 10 most recent messages and photos, so the wall stays fresh as new guests sign in.

Features
Feature	Korean UI label	Description
Message canvas	메세지 작성하기	Freehand writing area for the guest's message
Ribbon colors	깃발 색상	Seven ribbon colors to pick before writing
Drawing tools	필기도구	Pencil, marker and brush, with four stroke sizes and nine colors
Undo / redo	(arrow buttons)	Step back or forward through strokes
Rewrite	다시쓰기	Clear the canvas and start again
Stickers	(emoji panel)	Ten emoji and reaction stickers to attach
Photo capture	사진 찍기 / 사진찍기	Take a photo with the webcam
Retake	다시찍기	Discard the photo and take a new one
Submit	등록하기	Publish the message and photo
Big-screen wall	(display view)	Latest 10 entries shown as bubbles
Tech stack
Engine / framework: Unity (C#)
Storage: local files (no external database or server)
Platform: Windows touch kiosk
Hardware: webcam, touchscreen kiosk (input) and a second large display (output)
How it works
The app uses two screens: the touchscreen kiosk shows the input interface, and the large display shows the bubble wall.
Each submitted message, sticker choice and photo is saved as local files.
The bubble wall reads the 10 newest entries and renders them as floating bubbles.
When a new entry arrives, the oldest one drops off the screen.
Download and run

A Windows build is available under Releases. The source code is not published.

Download the latest .zip from the Releases page and extract it.
Connect a webcam (needed for the photo step).
Connect a second display for the bubble wall.
Run the .exe file.

Note: the floating message and photo bubbles appear only on the second display. With a single screen you will see the input interface but not the bubble wall.

Windows may show a "Windows protected your PC" (SmartScreen) warning because the app is not code-signed. Choose More info, then Run anyway. Only do this if you trust the source.

My role
Developed the guest input interface: drawing canvas, stickers and photo capture
Built the submission flow and the "latest 10" display logic
Handled deployment at the event on the touch kiosk
Privacy

The screenshot shows a test photo. Real guest messages and photos from the event are not included in this repository.

Credits

Built for a university anniversary event, February 2025.

License

All rights reserved. The source code is not published, and the executable is provided for demonstration only.
