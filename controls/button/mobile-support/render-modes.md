---
title: Render Modes
page_title: Render Modes | RadButton for ASP.NET AJAX Documentation
description: Render Modes
slug: button/mobile-support/render-modes
tags: render,modes
published: True
position: 3
---

# Render Modes

**RadButton** has two different render modes that can change the actual HTML markup that is rendered.	They are exposed via the **RenderMode** property that can have four	possible values - **Classic**, **Lightweight**, **Mobile** and **Auto**.	This functionality was introduced in the **Q1 2015** version.

The possible options are:

* **Classic**—this mode is the rendering that has been used before. It remains without changes and it is the default value of the property.	In this mode span elements and background images (in several sprites) are used to create the layout (including rounded corners, shadows, icons etc.).

* **Lightweight**—this mode emphasizes on semantic HTML and CSS3. It reduces the amount of markup the control renders	and makes it easier to customize. This also reduces the number of image sprites required by the control. All of this decreases the overall size and complexity of each skin, including custom ones.

* **Mobile**—this mode is currently not supported. If you set it, the mode will fall back automatically to **Lightweight**.

* **Auto**—this mode makes each control choose the appropriate rendering mode according to the used	browser—**Classic** or **Lightweight**. This functionality was added in Q1 2015.


@[template](/_templates/common/render-mode.md#do-not-mix-modes-buttons "control: RadButton")


## Setting Render Mode


@[template](/_templates/button/render-modes.md#set-render-mode)

## See Also

 * [Mobile Support Overview]({%slug button/mobile-support/overview%})

 * [Elastic Design]({%slug button/mobile-support/elastic-design%})

 * [Fluid Design]({%slug button/mobile-support/fluid-design%})
