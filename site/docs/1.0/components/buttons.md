---
layout: docs
title: Buttons
---

# Buttons

Use sentence case for text on buttons. The width of the button will depend on the text on the button. When placing text in buttons

- be concise
- do not use a long sentence
- use trigger words like Download, View or Print

Buttons should be aligned left and the left edge should align with the content on the page.

If links must be styled as buttons they should be calls to action, such as, Next, Start or Confirm.

> **IMPORTANT:**
> If you want to link users between pages of a website, use `<a class="btn" href="#"`, `<button class="btn"></button>` should be used for actions inside a form.

## Primary Buttons

In general, use primary buttons for actions that go to the next step

{% capture example %}
<button type="button" class="c-btn c-btn--primary">Primary button</button>
{% endcapture %}
{% include example.html content=example %}

{% capture snippet %}
<button type="button" class="c-btn c-btn--primary">
Primary button
</button>
{% endcapture %}
{% include snippet.html content=snippet %}

There are cases where certain actions require specific button styling. We deal with this by creating modifier classes. An example of this can be seen below for a previous button which requires slightly different colours to a primary button. In this instance we've created the `c-btn--action-prev` class.

{% capture example %}
<button type="button" class="c-btn c-btn--primary c-btn--action-prev">Previous</button>
<button type="button" class="c-btn c-btn--primary">Next</button>
{% endcapture %}
{% include example.html content=example %}

{% capture snippet %}
<button type="button" class="c-btn c-btn--primary c-btn--action-prev">
Previous
</button>
{% endcapture %}
{% include snippet.html content=snippet %}

## Secondary Buttons

Use secondary buttons for actions that happen on the same page.

{% capture example %}
<button type="button" class="c-btn c-btn--secondary">Secondary button</button>
{% endcapture %}
{% include example.html content=example %}

{% capture snippet %}
<button type="button" class="c-btn c-btn--secondary">
Secondary button
</button>
{% endcapture %}
{% include snippet.html content=snippet %}

## Icons in buttons

You should always place icons on the right of the button text. Use icons for specific actions for example Download, Print or Expand.

The exception is the previous button, which has an arrow pointing left to the left side of the text.

## Disabled buttons

Don’t disable buttons - unless there’s a good reason. For example, you could disable a button in a booking system if there are no bookings available.

You should give the user another way to continue - like by adding an error message or text to explain why the button is disabled

## Accessibility

Buttons should display a visible focus state when users tab to them Avoid using `<div>` or `<img>` tags to create buttons. Screen readers don’t automatically know either is a usable button.

When styling links to look like buttons, remember that screen readers handle links slightly differently than they do buttons. Pressing the Space key triggers a button, but pressing the Enter key triggers a link.

Use the aria-disabled attribute for older screen readers.